{
  "date" : "2022-01-23",
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"ملف GDOC - اختصار محرر مستندات Google" ,
  "description":"تعرف على ما هو ملف GDOC وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات GDOC وفتحها." ,
  "linktitle" : "GDOC",
  "menu" : {
    "docs" : {
      "parent" : "web"
}
} ,
  "lastmod" : "2022-01-23"
}

## ما هو ملف GDOC؟

ملف GDOC هو ملف اختصار يشير إلى ملف موجود على Google Drive ، وهي خدمة تخزين مستندات سحابية. عندما يتم تثبيت عميل Google Drive على جهاز كمبيوتر ويتم إنشاء مستند بداخله ، ينشئ محرك الأقراص مستندًا في التخزين السحابي عبر الإنترنت ويكتب [URL](/ar/web/url/) لهذا المستند في ملف GDOC في Google المحلي مجلد محرك الأقراص. عند النقر المزدوج على ملف الاختصار هذا ، يفتح مستعرض الويب الافتراضي المستند من موقع [URL](/ar/web/url/). إذا تم نقل ملف الاختصار هذا خارج هذا المجلد ، فسيتم قطع الارتباط إلى المستند عبر الإنترنت.

## تنسيق ملف GDOC - مزيد من المعلومات

يحتوي ملف GDOC على اختصار للمستند عبر الإنترنت المكتوب بتنسيق ملف [JSON](/ar/web/json/). يقوم المستعرض الذي يفتح ملفات GDOC بقراءة معلومات URL ويفتح المستند المرتبط للعرض بشرط أن يتم تسجيل دخول المستخدم إلى حساب Google هذا حيث يتم تخزين المستند. لا تحتوي ملفات GDOC على محتويات المستند.

### مثال ملف GDOC

يمكن فتح ملف GDOC في محرر نصوص وتبدو محتوياته كما يلي.

```
{"url": "https://docs.google.com/a/test.com/spreadsheet/ccc?key=01234567898765432123456789&usp=docslist_api", "resource_id": "spreadsheet:0A12345B678HJK9TZPL9078767"}
```

كما يمكن رؤيته ، يتم تنسيق المحتويات في JSON مع وجود عنوان URL للمستند ومعرف المستند المرتبط.

## مراجع

* [محرر مستندات Google لا يفتح ملفات gdoc أو docx](https://support.google.com/docs/thread/8408691/google-docs-not-opening-either-gdoc-or-docx-files؟hl=ar )

