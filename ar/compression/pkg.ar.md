{
  "date" : "2021-04-08",
  "keywords" :["ملف pkg" , "تنسيق ملف pkg" , "ما هو ملف pkg" , "ملف" , "مثال pkg" , "امتداد ملف pkg" , "امتداد" , "تنسيق"] ,
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"PKG - تنسيق ملف الأرشيف القابل للتوسيع" ,
  "description":"تعرف على تنسيق ملف PKG وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات PKG وفتحها." ,
  "linktitle" : "PKG",
  "menu" : {
    "docs" : {
      "parent" : "compression"
}
} ,
  "lastmod" : "2021-04-13"
}

## ما هو ملف PKG؟

الملف بامتداد .pkg هو ملف حزمة مثبت يُستخدم لتثبيت البرنامج على نظام التشغيل macOS. بالإضافة إلى أجهزة كمبيوتر Macintosh ، يتم استخدامه على iPhone أيضًا. يمكن استخدام تطبيق مثبت Apple المدمج لتثبيت محتويات ملف PKG. ملف PKG مشابه لملف MSI المستخدم على نظام تشغيل Windows لتثبيت البرنامج. أثناء التثبيت ، يمكن لملفات الحزمة هذه تسجيل الرسائل التي تمنحك فكرة عن الأشياء الإضافية التي تم تثبيتها بواسطة هذه الحزمة.

## تنسيق ملف PKG

PKR هي ملفات ثنائية يتم ضغطها لتقليل الحجم الكلي للملف. منذ OSX 10.5 ، قدمت Apple الحزم المسطحة مع ملفات التثبيت الفردية. هذه مختلفة عن تنسيقات الحزم السابقة التي جاءت كحزم بدلاً من ملفات فردية. تحتوي هذه الحزم المجمعة على تسلسل هرمي مهيكل للدليل يقوم بتخزين الملفات بطريقة تسهل استرجاعها عبر بعض ملفات الفهرس. تنسيق ملف PKG المسطح هو في الواقع أرشيف [XAR](/ar/compression/xar/) يحتوي على:

* رأس - يحدد الحجم ، المجموع الاختباري ، ومعلومات الإصدار
* جدول المحتويات - مستند XML (ويجب) ترميزه كـ UTF-8 ويتم تخزينه في بداية الملف ، مما يجعل من السهل المسح عبر الأرشيف لاستخراج ملف فردي
* كومة - كومة غير منظمة من البيانات المشار إليها بواسطة جدول المحتويات

## مراجع

* [تنسيق ملف حزمة مسطح](http://s.sudre.free.fr/Stuff/Ivanhoe/FLAT.html)
* [PKG - Wikipedia](https://en.wikipedia.org/wiki/.pkg)

