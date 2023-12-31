{
  "date" : "2021-06-30",
  "keywords" :["ملف exe" , "تنسيق ملف exe" , "ما هو ملف exe" , "ملف" , "مثال" , "امتداد ملف exe" , "امتداد" , "تنسيق"] ,
  "author" : {
    "display_name" : "Muhammad Umar"
} ,
  "draft" : "false",
  "toc" : true,
  "description":"ملف. exe هو ملف Microsoft قابل للتنفيذ يتم تشغيله على نظام تشغيل Windows. تعرف على المزيد حول تنسيق ملف EXE." ,
  "title" :"ما هو ملف EXE القابل للتنفيذ؟" ,
  "linktitle" : "EXE",
  "menu" : {
    "docs" : {
      "parent" : "executable"
}
} ,
  "lastmod" : "2021-06-30"
}

## ما هو ملف EXE؟

كلمة EXE هي اختصار لـ ** قابل للتنفيذ **. ملف. exe هو برنامج يمكن تنفيذه على نظام التشغيل Microsoft Windows. يقوم مطورو التطبيقات في الغالب بنشر برامجهم لنظام التشغيل Windows بتنسيق قابل للتنفيذ كملفات exe. إنه تنسيق الملف القياسي لتشغيل التطبيقات على Windows. ** Setup.exe ** و ** Install.exe ** و ** cmd.exe ** هي بعض الأسماء الشائعة والمألوفة لملفات EXE.

## تنسيق ملف EXE

تم تقديم برامج التحويل البرمجي لـ MS-DOS مع نماذج الذاكرة ذات الحد من الذاكرة 64 كيلو بايت. المفهوم العام هو تعيين سجلات قطاعات مختلفة في وحدة المعالجة المركزية x86 (CS ، DS ، ES ، SS) للإشارة إلى الأجزاء المختلفة أو نفسها ، وبالتالي السماح بدرجات مختلفة من الوصول إلى الذاكرة. بعض نماذج الذاكرة المحددة هي:

- ** Tiny **: جميع عمليات الوصول إلى الذاكرة 16 بت (لم تتغير تسجيلات المقطع). ينتج ملف .COM بدلاً من ملف .EXE.
- ** صغير **: جميع عمليات الوصول إلى الذاكرة 16 بت (لم تتغير تسجيلات المقطع).
- ** مضغوط **: تتضمن عناوين البيانات كلاً من المقطع والإزاحة ، وإعادة تحميل سجلات DS أو ES عند الوصول والسماح لما يصل إلى مليون من البيانات. لا تؤدي عمليات الوصول إلى التعليمات البرمجية إلى تغيير سجل CS ، مما يسمح بـ 64 كيلو بايت من التعليمات البرمجية.
- ** متوسط **: تتضمن عناوين الكود عنوان المقطع وإعادة تحميل CS عند الوصول والسماح لما يصل إلى مليون رمز. لا تؤدي عمليات الوصول إلى البيانات إلى تغيير سجلات DS و ES ، مما يتيح 64 كيلو بايت من البيانات.
- ** كبير **: كل من عناوين الرموز والبيانات هي أزواج (جزء ، إزاحة) ، يتم دائمًا إعادة تحميل عناوين المقطع. مساحة الذاكرة كاملة 1 ميغا بايت متاحة لكل من التعليمات البرمجية والبيانات.
- ** ضخم **: مثل النموذج الكبير ، مع حساب إضافي يتم إنشاؤه بواسطة المترجم للسماح بالوصول إلى المصفوفات الأكبر من 64 كيلو بايت.

يجب على المطورين تحديد النموذج الذي يجب تحديده أثناء إنشاء ملف exe.

### تنسيق ملف EXE المحمول

يحتوي تنسيق الملف القابل للتنفيذ المحمول (PE) على عدد من رؤوس المعلومات ، فيما يلي قائمة الرؤوس:

- ** رأس DOS **: يضمن رأس MS-DOS التوافق مع الإصدارات السابقة أو الرفض الرائع لأنواع الملفات الجديدة.
- ** رأس PE **: عند الإزاحة 60 (0x3C) من بداية رأس DOS هو مؤشر إلى رأس ملف PE
- ** COFF Header **: يحتوي رأس COFF على بعض المعلومات المفيدة للملف القابل للتنفيذ ، وبعض المعلومات الأكثر فائدة لملف الكائن.
- ** رأس اختياري PE **: يحدث رأس PE الاختياري مباشرةً بعد رأس COFF ، بل إن بعض المصادر تعرض الرأسين على أنهما جزء من نفس البنية.
- ** جدول القسم **: مباشرة بعد رأس PE الاختياري نجد جدول قسم. يتكون جدول القسم من صفيف من هياكل IMAGE_SECTION_HEADER.
- ** الأقسام القابلة للتخطيط **: يمكن توفير مساحة في الذاكرة عن طريق تعيين رمز مكتبة في أكثر من عملية.

## هل يمكنك تشغيل ملف EXE على جهاز Mac؟

لا يتم استخدام ملفات Exe كملفات قابلة للتنفيذ على نظام التشغيل Mac OS. ومع ذلك ، إذا كنت تريد تشغيل ملف exe على نظام التشغيل Mac OS ، فيمكن استخدام الطرق التالية.

1. ** Wine ** - Wine هو الحل الأمثل للأشخاص الذين يرغبون في استخدام تطبيقات الكمبيوتر الخاصة بهم على أنظمة Mac. إنه اختصار يرمز إلى "Wine Is Not A Emulator" بمعنى. يقوم Wine بإنشاء نفس بيئة الدلائل التي تستخدمها Microsoft حتى تتمكن من تشغيل تطبيق Windows الخاص بك باستخدامه.
2. ** الأجهزة الافتراضية ** - أنشئ جهازًا افتراضيًا يعمل بنظام Windows باستخدام Parallel Desktop أو VM Virtual Box وقم بتشغيل التطبيق الخاص بك داخل الجهاز الظاهري.
3. ** Boot Camp ** - يتيح لك تثبيت Windows Boot Camp وتكوينه على نظام Mac OS تشغيل نظام التشغيل Windows على جهاز Mac.

## مراجع

* [.exe- بواسطة Wikipewdia](https://en.wikipedia.org/wiki/.exe)
* [x86 Disassembly / Windows Executable Files](https://en.wikibooks.org/wiki/X86_Disassembly/Windows_Executable_Files#MS-DOS_EXE_Files)

