{
  "date" : "2022-06-29",
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"تنسيق ملف WHL - ملف حزمة Python Wheel" ,
  "description":"تعرف على تنسيق ملف WHL وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات WHL وفتحها." ,
  "linktitle" : "WHL",
  "menu" : {
    "docs" : {
      "parent" : "compression"
}
} ,
  "lastmod" : "2022-06-29"
}

## ما هو ملف WHL؟

ملف WHL (Wheel) هو ملف حزمة توزيع محفوظ بتنسيق عجلة Python. إنه تثبيت تنسيق قياسي لتوزيعات Python ويحتوي على جميع الملفات والبيانات الوصفية المطلوبة للتثبيت. يحتوي ملف WHL أيضًا على معلومات حول إصدارات Python والأنظمة الأساسية التي يدعمها ملف العجلة هذا. على غرار ملف إعداد [MSI](/ar/executable/msi/) ، تنسيق ملف WHL هو تنسيق جاهز للتثبيت يسمح بتشغيل حزمة التثبيت دون إنشاء توزيع المصدر.

## تنسيق ملف WHL

تنسيق ملف WHL هو [ZIP](/ar/compression/zip/) (.zip) أرشيف يحتوي على جميع ملفات التثبيت والبيانات الوصفية المطلوبة من قبل المثبتين لتثبيت الحزمة. يمكن استخراج ملفات WHL باستخدام خيار فك الضغط أو تطبيقات برامج فك الضغط القياسية مثل WinZIP و WinRAR.

### اصطلاح اسم ملف WHL

يتم تسمية ملف WHL وفقًا للاتفاقية التالية.

```
{dist}-{version}(-{build})?-{python}-{abi}-{platform}.whl
```

مثال على اسم ملف WHL كما يلي.

```
cryptography-2.9.2-cp35-abi3-macosx_10_9_x86_64.whl
```

* "التشفير" هو اسم الحزمة.
* "2.9.2" هو إصدار الحزمة الخاص بالتشفير. الإصدار عبارة عن سلسلة متوافقة مع PEP 440 مثل 2.9.2 أو 3.4 أو 3.9.0.a3.
* `cp35` هو علامة Python ويشير إلى تطبيق Python والإصدار الذي تتطلبه العجلة.
* "abi3" هي علامة ABI. ABI تعني الواجهة الثنائية للتطبيق.
* `macosx_10_9_x86_64` هي علامة النظام الأساسي ، والتي تصادف أنها مليئة بالفم.

## مراجع

* [ما هي عجلات Python ولماذا يجب أن تهتم؟](https://realpython.com/python-wheels/)
* [عجلة بايثون](https://pypi.org/project/wheel/)

