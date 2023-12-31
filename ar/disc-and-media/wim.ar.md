{
  "date" : "2021-08-11",
  "keywords" :["wim file", "wim file format", "what is a wim file", "file", "wim example", "wim file extension", "extension", "format"],
  "author" : {
    "display_name" : "Muhammad Umar"
} ,
  "draft" : "false",
   "toc" : true,
  "description" :"تعرف على تنسيق ملف WIM وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات WIM وفتحها." ,
  "title" :"WIM - ملف تنسيق صور Windows" ,
  "linktitle" : "WIM",
  "menu" : {
    "docs" : {
      "parent" : "disc-and-media"
}
} ,
  "lastmod" : "2021-08-11"
}

## ما هو ملف WIM؟
شوهدت الملفات ذات الامتدادات wim. لأول مرة في Windows Vista. ينتمي WIM إلى تنسيق تصوير قائم على الملفات والذي تم تقديمه عادةً في نظام التشغيل Microsoft Windows Vista. إنه يتيح نشر صورة قرص واحد على العديد من منصات الكمبيوتر. تُستخدم ملفات WIM لإدارة الملفات مثل التحديثات وبرامج التشغيل والمكونات دون إعادة تمهيد صورة نظام التشغيل. يحتوي ملف AQ WIM على مجموعة من الملفات والبيانات الوصفية المرتبطة بها والتي تشبه إلى حد بعيد تنسيقات ملفات القرص الأخرى.

## تنسيقات ملفات WIM
لا يشبه تنسيق ملف WIM التنسيقات القطاعية مثل VHD أو IS ، فهو في الواقع مستند إلى ملف مما يعني أن الوحدة الأساسية للمعلومات في WIM هي ملف. الميزة الأساسية لكونها قائمة على الملفات هي تخزين نسخة واحدة من ملف تمت الإشارة إليه عدة مرات في شجرة نظام الملفات واستقلالية الأجهزة ، مما يقلل من عبء فتح وإغلاق الملفات المختلفة بشكل فردي ، لأن الملفات يتم تخزينها داخل WIM واحد. ملف. يمكن لملفات WIM تخزين صور متعددة للقرص ، والتي يشار إليها إما باسمها الفريد أو من خلال فهرسها العددي.
### دعم خوارزميات الضغط
يدعم WIM العائلات التالية من خوارزميات الضغط بسرعة تنازلية ونسبة تصاعدية:
- XPRESS
- LZX
- LZMS
- ضغط صلب.
تعتمد العائلات الثلاث الأولى على LZ77 بينما تم تقديم الضغط الصلب جنبًا إلى جنب مع LZMS في WIMGAPI Windows 8 و DISM Windows 8.1.
### أدوات لتنسيق ملف WIM
عادة ما تدعم الأدوات التالية تنسيق ملف WIM:

- ** ImageX **: أداة سطر أوامر تُستخدم لتحرير وإنشاء ونشر صور قرص Windows بتنسيق Windows Imaging Format. إلى جانب WIMGAPI ذي الصلة ، يتم توزيعه كجزء من مجموعة أدوات التثبيت التلقائي لنظام التشغيل Windows. بدءًا من Windows Vista ، يستخدم برنامج إعداد Windows WAIK API لتثبيت Windows.
- ** DISM **: أداة مقدمة في Windows 7 و Windows Server 2008 R2 يمكنها أداء المهام المتعلقة بالخدمة على صورة تثبيت Windows ، سواء كانت صورة عبر الإنترنت أو صورة غير متصلة بالإنترنت داخل مجلد أو ملف WIM. كانت هذه الأداة قادرة على تركيب الصور وإلغاء تركيبها ، وإضافة برنامج تشغيل للجهاز إلى صورة غير متصلة بالإنترنت والاستعلام عن برامج تشغيل الأجهزة المثبتة في صورة غير متصلة بالإنترنت.
 




## مراجع


* [Windows Imaging Format - بواسطة Wikipedia](https://en.wikipedia.org/wiki/Windows_Imaging_Format)


