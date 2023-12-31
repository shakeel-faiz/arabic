{
  "date" : "2021-03-08",
  "keywords" :["RB", "Nuvo Media's Rocket eBook device", "file", "extension", "format", "eBook"],
  "author" : {
    "display_name" : "Muhammad Umar"
} ,
  "draft" : "false",
  "toc" : true,
  "description":"تعرف على تنسيق ملف RB لجهاز Nuvo Media's Rocket eBook و APIs التي يمكنها إنشاء ملفات RB وفتحها." ,
  "title" :"RB - Rocket eBook File",
  "linktitle" : "RB",
  "menu" : {
    "docs" : {
      "parent" : "ebook"
}
} ,
  "lastmod" : "2021-03-08"
}

## ما هو ملف RB؟

يحتوي الملف بامتداد .rb على محتوى Rocket eBook. إن Rocket eBook هو في الواقع جهاز تم تصنيعه بواسطة Nuvo Media ؛ أطلقوا هذا الجهاز في عام 1998. على الرغم من أن Rocket eBook قادر على عرض الصور ، ولكن فقط في عرض أبيض وأسود. لديها شاشة 106 نقطة في البوصة أو 480 × 320 بكسل على شاشة تعمل باللمس 4.5 × 3 بوصة. يتصل Rocket eBook بجهاز كمبيوتر عبر اتصال منفذ تسلسلي لتنزيل الكتب الإلكترونية بتنسيق ملف RB. يمكن لملفات RB استخدام DRM ولكن لا يتم استخدام هذه التقنية في الكتب الإلكترونية الحديثة. يحتوي ملف RB بشكل تقليدي على ملف HTML مع الصور وملف pseudo-OPF مع جميع البيانات الوصفية (.info).

## المواصفات الفنية لتنسيق ملف RB ##

يظهر رقم سحري (في شكل سداسي عشري) في أول 4 بايت للملف: B0 0C B0 0C.

يبدو أن البايتين التاليين هما رقم إصدار ، مثل "02 00" ، والذي يرمز إلى الإصدار الرئيسي 2 والإصدار الثانوي 0.

تحتوي البايت الأربعة التالية على النص "NUVO" ، متبوعًا بـ 4 بايت من 00h.

4 بايت التالية هي تاريخ إنشاء الكتاب ، وتم ترميزها كـ int16. هذا يضعنا في تعويض 0Eh. قامت النسخة القديمة من ORocketLibrary بترميز القيمة الكاملة للسنة (على سبيل المثال ، 1999 كانت "CF 07" ، 2000 كانت "D0 07"). في الإصدار الأخير ، يتم تخزين tm_year حرفيًا ، أي 100 لعام 2000 ("64 00"). بعد السنة تأتي int8 تمثل رقم الشهر ذي الصلة ، و int8 تمثل يوم الشهر.

6 بايت التالية هي 00 h. لضبط الوقت ، قد تكون محجوزة.

يتم تضمين الإزاحة المطلقة لـ "جدول المحتويات" في int32 عند الإزاحة 18 ساعة.

بعد ذلك يوجد int32 يحتوي على طول ملف .rb. يستخدم هذا لتحديد ما إذا كانت الملفات كاملة أم لا.

يبدو أن هذا الجزء الكامل من البايتات (من 20 ساعة إلى 128 ساعة) مطلوب فقط من خلال عنوان مشفر. في العناوين غير المشفرة ، تكون دائمًا صفرية.

في معظم الحالات ، يتبع جدول المحتويات (عند الإزاحة 128). يبدأ بعدد int32 لعدد إدخالات "الصفحة" (أقسام ملف .rb) في ToC. يتكون كل إدخال من اسم (صفر مبطن حتى 32 بايت) ، متبوعًا بـ 3 وحدات int32: طول مقطع البيانات ، والموضع في ملف .rb ، وعلامة لهذا الإدخال. اعتبارًا من اليوم ، القيم المعروفة هي: 1 (مشفرة) ، 2 (صفحة معلومات) ، و 8 (مفرغة). تم تصميم جميع الأسماء ، حسب الضرورة ، للتأكد من أنها كلها فريدة من نوعها.

## مراجع

* [قارئ إلكتروني - بواسطة MobileRead](https://en.wikipedia.org/wiki/E-reader)

