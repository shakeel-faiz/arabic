{
  "date" : "2021-07-15",
  "keywords" :["LNK", "extension", "file", "format", "system", "LNK file", "link", "LNK files", "LNK documents", "application", "programmes"],
  "author" : {
    "display_name" : "Sami Cheema"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"LNK - تنسيق ملف الارتباط" ,
  "description":"تعرف على تنسيق ملف LNK وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات LNK وفتحها." ,
  "linktitle" : "LNK",
  "menu" : {
    "docs" : {
      "parent" : "system"
}
} ,
  "lastmod" : "2021-07-15"
}

## ما هو ملف LNK؟ ##

ملف LNK ، الذي يماثل هوية على نظام Mac ، هو بديل لـ Windows أو "رابط" يعمل كوصلة لمجلد أو برنامج صورة أصلي. يحتوي على نوع وجهة الاختصار وموضعها واسم ملفها ، بالإضافة إلى التطبيق الذي يفتح المستند الهدف ومفتاح اختصار إضافي.

في Windows ، مباشرة ملف أو مجلد أو برنامج قابل للتنفيذ واختر إنشاء اختصار. يعد موقع تنسيق الملف ودليل "البداية" ميزتين أساسيتين لملفات LNK. يتم إخفاء تنسيق ملف ملفات LNK ، ويشير سهم منحني إلى أنها اختصارات.

## تنسيق ملف LNK ##

عادةً ما تحتوي تنسيقات ملفات LNK على نفس رمز ملفات الوجهة الخاصة بها ، ولكن مع إضافة سهم مجعد صغير لإظهار أن الملف يشير إلى موقع مختلف. عندما يتم النقر على الاختصار نقرًا مزدوجًا ، فإنه يتصرف كما لو أن المستخدم قد نقر نقرًا مزدوجًا فوق الملف الفعلي.

يمكن أن تحتوي ملفات LNK التي تحتوي على اختصارات للتطبيق على خصائص تؤثر على كيفية تشغيل البرنامج. لتغيير السمات ، انقر بزر الماوس الأيمن فوق ملف الاختصار واختر ** خصائص ** ، ثم قم بتغيير الحقل الهدف.

بدلاً من أن تكون امتدادات للملفات ، فإن ملفات LNK هي امتدادات Windows Explorer. كملحق طرفي ، لا يمكن استخدام مستندات .lnk إلا في Windows Explorer لاستبدال ملف ، ولها أغراض أخرى في Windows Explorer إلى جانب العمل كاختصار لمستند محلي. تبدأ هذه الملفات بالحرف "L" أيضًا.

بينما ترتبط الاختصارات بملفات وأدلة معينة عند إنشائها ، فقد تصبح غير قابلة للتشغيل إذا تم تغيير الهدف إلى موقع مختلف. سيبدأ Explorer في إصلاح مجلد اختصار يشير إلى هدف ميت عند فتحه.


## مواصفات تكنيكال ##

فقط عندما يتم إلغاء تحديد إعداد عرض المجلد "إخفاء الامتدادات لأنواع الملفات المعروفة" ، لا يُظهر Windows امتداد المستند .lnk لاختصارات المستندات. بينما لا ينصح بذلك ، يمكنك تمكين عرض امتداد الملف عن طريق إزالة خاصية "NeverShowExt" من عنصر تسجيل Windows HKEY_CLASSES_ROOT \ lnk file.

للقيام بذلك ، اتبع الخطوات التالية:

* افتح "محرر التسجيل" عن طريق إدخال "Regedit" في حقل البحث بشريط المهام واختيار البرنامج
* في التطبيق ، انتقل إلى موقع Computer \ HKEY HKEY_CLASSES_ROOT \ lnkfile
* قم بعمل نسخة احتياطية من العنصر بالنقر بزر الماوس الأيمن فوقه واختيار تصدير
* حدد وحذف السمة "NeverShowExt"
* يجب إعادة تشغيل Windows


## المرجعي ##

* [LNK - Wikipedia](https://en.m.wikipedia.org/wiki/Shortcut_(computing))
