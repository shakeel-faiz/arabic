{
  "date" : "2019-12-10",
  "keywords" :["XLM", "file", "extension", "file format", "Microsoft Excel Macro File", "Spreadsheet"] ,
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "description" :"دليل تنسيق الملف الخاص بك لمعرفة ما هو ملف XLM Macros و APIs التي يمكنها إنشاء ملفات XLM وفتحها." ,
  "title" :"ما هو ملف XLM؟" ,
  "linktitle" : "XLM",
  "menu" : {
    "docs" : {
      "parent" : "spreadsheet"
}
} ,
  "lastmod" : "2019-12-10"
}

## ما هو ملف XLM؟

يعد XLM ، لـ Excel Macro ، نوعًا من ملفات جداول البيانات المستخدمة لتخزين وحدات الماكرو. من وجهة نظر التطبيق ، الماكرو عبارة عن مجموعة من الإرشادات التي يتم استخدامها لأتمتة العمليات. يتم استخدام الماكرو لتسجيل الخطوات التي يتم إجراؤها بشكل متكرر لتنسيق ملف [XLS](/ar/ spreadsheet / xls /) ويسهل تنفيذ الإجراءات عن طريق تشغيل الماكرو مرة أخرى. تتم برمجة وحدات الماكرو باستخدام Microsoft Visual Basic للتطبيقات (VBA) من داخل Excel Workbook باستخدام محرر Visual Basic ويمكن تشغيل / تصحيح الأخطاء مباشرة من هناك.

## نبذة تاريخية ##

دعم Microsoft Excel برمجة وحدات الماكرو منذ أول إطلاق عام لها. ظلت ميزات وحدات الماكرو كما هي من خلال الإصدارات اللاحقة من Excel مع التمديد حسب الميزات الجديدة. كانت XLM لغة الماكرو الافتراضية لبرنامج Excel من خلال Excel 4.0. قام Excel 5.0 بتسجيل وحدات الماكرو في VBA افتراضيًا ولكن مع الإصدار 5.0 ، كان لا يزال يُسمح بتسجيل XLM كخيار. بعد الإصدار 5.0 توقف هذا الخيار. جميع إصدارات Excel ، بما في ذلك Excel 2010 قادرة على تشغيل ماكرو XLM ، على الرغم من أن Microsoft لا تشجع استخدامها.

## تسجيل ماكرو في XLM ##

يوفر Excel خطوات سهلة الاستخدام لتسجيل ماكرو. يتطلب أن يكون لديك أدوات مطور مثبتة للعمل مع وحدات الماكرو. بمجرد أن يتم تسجيل الماكرو ، فإنه يسجل كل إجراء للمستخدم ليتم تشغيله لاحقًا. يتضمن تسجيل الماكرو في الواقع جميع الخطوات التي يقوم بها المستخدم بعد بدء التسجيل. وبالتالي ، إذا جعلت محتوى الخلية غامقًا ومائلًا وقمت بتعيين ضبط النص الخاص بها بعد بدء تسجيل الماكرو ، فسيتم تسجيل كل هذه الأوامر. يمكن تعيين اختصار لكل ماكرو مسجل للتشغيل السريع لاحقًا. ينشئ تسجيل الماكرو تعليمات برمجية لـ VBA في شكل ماكرو يمكن تحريره باستخدام محرر Visual Basic (VBE).

## نموذج كائن Excel ##

تستخدم وحدات الماكرو إجراءات VBA في الخلف وتتبع [Excel Object Model](https://docs.microsoft.com/en-us/office/vba/api/overview/excel/object-model) لهذا الغرض. يحدد هذا النموذج كائنات جدول البيانات للتفاعل مع جدول البيانات من خلال أشرطة أدوات الأوامر المحددة من قبل المستخدم أو أشرطة الأوامر أو مربعات الرسائل. على سبيل المثال ، يتم منح الوصول إلى خصائص المصنف من خلال كائن المصنف. وبالمثل ، يوجد كائن ورقة عمل في النموذج للعمل مع أوراق عمل المصنف برمجيًا.

## وحدات الماكرو والأمان ##

يسمح VBA بالوصول إلى جميع مجالات التطبيق بالإضافة إلى نظام الملفات ويمكن أن يكون خطيرًا أيضًا. يثير هذا مخاوف عند مشاركة المصنف مع شخص يمكنه تشغيل الملف في نهايته. هذا هو Microsoft Excel يحذر من فتح مثل هذا الملف. يمكن اعتماد وحدات الماكرو بتوقيع رقمي حتى يتمكن المستخدمون الآخرون من التحقق من أنها جديرة بالثقة. وبالتالي ، يمكن تمكين وحدات الماكرو بعد التحقق من مصدرها.

## مراجع ##

* [[MS-XLS] - بنية تنسيق ملف Excel الثنائي](https://msdn.microsoft.com/en-us/library/cc313154 (v # office.12) .aspx)
* [برمجة ماكرو](https://en.wikipedia.org/wiki/Microsoft_Excel#Macro_programming)
