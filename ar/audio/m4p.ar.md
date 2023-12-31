{
  "date" : "2021-06-09",
  "keywords" :["m4p" , "mp3" , "ملف" , "امتداد" , "تنسيق" , "ما هو تنسيق ملف m4p" , "موسيقى" , "تنسيق ملف m4p" , "M4b مقابل MP3" , "مواصفات تنسيق ملف m4p "] ,
  "author" : {
    "display_name" : "Muhammad Umar"
} ,
  "draft" : "false",
  "toc" : true,
  "description" :"تعرف على تنسيق ملف M4P وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات M4P وتحويلها وفتحها." ,
  "title" :"تنسيق ملف الكتاب المسموع M4P - MPEG-4" ,
  "linktitle" : "M4P",
  "menu" : {
    "docs" : {
      "parent" : "audio"
}
} ,
  "lastmod" : "2021-06-09"
}

## ما هو ملف M4P؟
الملف بامتداد .m4p هو ملف صوتي يتوفر عادة في متجر Apple iTunes للتنزيل. بعبارة أخرى ، يمكننا القول أن M4P هو ملف AAC ولكنه محمي ضد النسخ باستخدام إدارة الحقوق الرقمية (DRM). هذا يعني أنه لا يمكن تشغيل ملفات M4P إلا على الأنظمة أو الأجهزة المعتمدة. عادةً ما تكون ملفات M4P خاصة بأجهزة الوسائط المتعددة من Apple. لذلك لا يمكن تشغيل هذه الملفات إلا على أجهزة Apple macbooks ، والبودكاست ، والهواتف الذكية مثل iPhone 6 أو iPhone 7.

## تنسيق ملف M4P
يرمز M4P إلى MPEG 4 Protected (صوتي) ، ويقوم بترميز الصوت باستخدام برنامج ترميز الصوت المتقدم (AAC) ويحمي الملف من الاستخدام غير المصرح به للملف. يُعتبر تنسيق الملف هذا عادةً تنسيق ملف صوتي في iTunes Music Store. تستخدم Apple نظام FairPlay Digital Rights Management (DRM) لحماية ملفات M4P. يعتمد FairPlay DRM على تقنية طورتها شركة Veridisc. تعمل آلية الحماية الخاصة به عن طريق تشفير دفق الصوت AAC باستخدام تشفير AES. يتلقى المستخدم مفتاحًا رئيسيًا مخصصًا لحسابه لفك التشفير. تم تقديم تنسيق الملف هذا كبديل لتنسيق ملف MP3 ، لأنه لم يكن المقصود من MP3 في الأصل أن يكون ملفًا صوتيًا ، ولكن كطبقة ثالثة في ملف فيديو MPEG 1 أو 2.


## مواصفات تنسيق ملف M4P

على غرار [M4A](/ar/audio/m4a/) ، تتكون ملفات M4P أيضًا من أجزاء متتالية. كل قطعة لها رأس 8 بايت ومقسمة فرعيًا على النحو التالي:
- حجم القطعة 4 بايت (كبير النهاية ، البايت العالي أولاً)
- نوع مقطع 4 بايت - أحد التوقيعات المحددة مسبقًا: "mdat" ، "moov" ، "pnot" ، "moof" ، "udta" ، "uuid" ، "free" ، "skip" ، "ftyp" ، "jP2" ، "عريض" ، "تحميل" ، "imap" ، "مات" ، "chap" ، "kmat" ، "clip" ، "crgn" ، "sync" ، "tmcd" ، "PICT" ، "scpt "،" ctab "،" ssrc ".

على غرار M4A ، سيكون الجزء الأول في M4P من النوع "ftype" وله نوع فرعي عند الإزاحة 8. يتم تعريف M4P بواسطة النوع الفرعي والذي يجب أن يكون "M4P_".

تكرار القطع ، حتى يتم اكتشاف جزء من نوع غير معروف ، سيقوم بتكوين ملف M4P (MPEG-4 Audio).

## مراجع ##

* [MPEG-4 الجزء 14 - بواسطة ويكيبيديا](https://en.wikipedia.org/wiki/MPEG-4_Part_14)
* [MPEG-4 Part 14 Audio (M4A، M4B، M4P) مثال على التنسيق والاسترداد](https://www.file-recovery.com/m4a-signature-format.htm)

