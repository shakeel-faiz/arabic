---
date: 2019-10-11
keywords: json , .json , تنسيق ملف json , كيفية فتح ملفات json , تدوين كائن javascript , تنسيق بيانات json , تنسيق ملف json.
مؤلف:
  display_name: Muhammad Ahmad Chishti
draft: false
toc: true
title: تنسيق ملف JSON - ما هو ملف JSON؟
linktitle: JSON
description: "تعرف على تنسيق ملف JSON وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات JSON وفتحها."
menu:
  docs:
    parent: "web"
lastmod: 2020-04-12
---

## ما هو ملف JSON؟

JSON (JavaScript Object Notation) هو تنسيق ملف قياسي مفتوح لمشاركة البيانات التي تستخدم نصًا يمكن للبشر قراءته لتخزين البيانات ونقلها. يتم تخزين ملفات JSON بامتداد .json. يتطلب JSON تنسيقًا أقل وهو بديل جيد لـ [XML](/ar/web/xml/). JSON مشتق من JavaScript ولكنه تنسيق بيانات مستقل عن اللغة. يتم دعم إنشاء وتحليل JSON من قبل العديد من لغات البرمجة الحديثة. * application / json * هو نوع الوسائط المستخدم لـ JSON.

## تنسيق ملف JSON - نبذة تاريخية

كانت هناك حاجة إلى خادم في الوقت الفعلي لاتصالات العميل التي أدت إلى إنشاء JSON. تم تحديد تنسيق JSON لأول مرة بواسطة دوجلاس كروكفورد في مارس 2001. استند JSON على الإصدار القياسي ECMA-262 الثالث - ديسمبر 1999 وهو مجموعة فرعية من JavaScript.

تم نشر الإصدار الأول من معيار ECMA-404 من JSON في أكتوبر 2013 بواسطة Ecma International. أصبح RFC 7159 المرجع الرئيسي لاستخدامات JSON للإنترنت في 2014. في نوفمبر 2017 ، تم نشر ISO / IEC 21778: 2017 كمعيار دولي. تم نشر RFC 8259 في 13 ديسمبر 2017 من قبل فريق عمل هندسة الإنترنت وهو الإصدار الحالي من معيار الإنترنت STD 90.

## هيكل ملف JSON

تتم كتابة بيانات JSON في أزواج ** مفتاح / قيمة **. يتم الفصل بين المفتاح والقيمة بنقطتين (:) في المنتصف مع وجود المفتاح على اليسار والقيمة على اليمين. يتم فصل أزواج المفاتيح / القيم المختلفة بفاصلة (،). المفتاح عبارة عن سلسلة محاطة بعلامات اقتباس مزدوجة على سبيل المثال "الاسم". يمكن أن تكون القيم من الأنواع التالية.

- "رقم"
- "String": تسلسل أحرف Unicode محاط بعلامات اقتباس مزدوجة.
- "قيمة منطقية": صواب أم خطأ.
- "مصفوفة": قائمة قيم محاطة بأقواس مربعة ، على سبيل المثال

"" json
["Apple" ، "Banana" ، "Orange"]
""

- "الكائن": مجموعة من أزواج المفاتيح / القيم المحاطة بأقواس معقوفة ، على سبيل المثال

"" json
{"الاسم": "جاك"، "العمر": 30، "مفضل سبورت": "كرة القدم"}
""

يمكن أيضًا أن تتداخل كائنات JSON لتمثيل بنية البيانات. فيما يلي مثال على كائن JSON.

### مثال على تنسيق JSON

```json
{
   "name":"Jack",
   "age":30,
   "contactNumbers":[
      {
         "type":"Home",
         "number":"123 123-123"
      },
      {
         "type":"Office",
         "number":"321 321-321"
      }
   ],
   "spouse":null,
   "favoriteSports":[
      "Football",
      "Cricket"
   ]
}
```

## ما هو الحجم الأقصى لملف JSON؟

لا يوجد حد عمليًا على الحد الأقصى لحجم ملف JSON. يمكن أن يكون طالما المساحة التي تتطلبها المحتويات ليتم تخزينها.

عندما يتعلق الأمر باستخدام تنسيق ملف JSON لنقل البيانات عبر الإنترنت ، يحتاج المرء إلى توخي الحذر بشأن الموارد المتاحة للكمبيوتر. إذا تم نقل بيانات JSON كبيرة ، فسوف يتأثر النقل إذا كانت ذاكرة متصفح العميل محدودة.


لا يوجد حد صارم محدد بالمواصفات ، ولكن يجب أن تكون حريصًا على عدم استنفاد الموارد على أجهزة كمبيوتر المستخدمين ، حيث سيؤدي ذلك إلى تدهور تجربة المستخدم بسرعة ، ومن المرجح أن يتخلوا عن تطبيقك.

## JSON مقابل XML

** XML ** هو تنسيق ملف آخر شائع ومستخدم على نطاق واسع لتبادل البيانات عبر الإنترنت. عندما يتعلق الأمر بتبادل البيانات بين التطبيقات ، فإن المطورين لديهم خيار استخدام كل من تنسيقات ملفات XML و JSON. ومع ذلك ، تم اعتماد JSON باعتبارها الطريقة الأكثر ملاءمة لتبادل البيانات بين التطبيقات عبر الإنترنت للأسباب التالية.

1. يوفر JSON عرضًا واضحًا وأسهل للقراءة للبيانات مقارنة بتنسيقات ملفات XML
1. يقلل JSON من عبء نقل البيانات عبر الإنترنت لأنه يحتوي على عدد أقل من الأحرف لتحديد نفس مجموعة البيانات مقارنةً بـ XML
1. توفر لغات البرمجة الحديثة محللات مضمنة لتحليل استجابة JSON عبر الويب.

## هل كنت تعلم؟

يمكنك أن تصبح مساهمًا في FileFormat.com للحفاظ على تحديث مجتمع تنسيق الملف بالنتائج التي توصلت إليها. إذا كان عليك مشاركة أي شيء حول JSON أو تنسيقات ملفات الويب ، فيمكنك نشر النتائج التي توصلت إليها في قسم [Web File Format News](https://news.fileformat.com/t/Web) حتى يتمكن الأشخاص من معرفة المزيد من هذه التنسيقات.

## مراجع

- [JSON - ويكيبيديا](https://en.wikipedia.org/wiki/CSS)
- [مقدمة إلى JSON](https://www.digitalocean.com/community/tutorials/an-introduction-to-json)

