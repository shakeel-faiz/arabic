{
  "date" : "2019-10-11",
  "keywords" :["ملف apng" , "تنسيق ملف apng" , "ما هو ملف apng" , "ملف" , "مثال apng" , "امتداد ملف apng" , "امتداد" , "تنسيق"] ,
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"تنسيق ملف APNG - ملف رسومات الشبكة المحمولة المتحركة" ,
  "description":"تعرف على تنسيق ملف APNG وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات APNG وفتحها." ,
  "linktitle" : "APNG",
  "menu" : {
    "docs" : {
      "parent" : "image"
}
} ,
  "lastmod" : "2020-09-10"
}

## ما هو ملف APNG؟

الملف ذو الامتداد .apng (الرسوم المتحركة للشبكة المحمولة) هو تنسيق رسومي نقطي وهو امتداد غير رسمي لـ Portable Network Graphic ([PNG](/ar/image/png/)). وهي تتألف من إطارات متعددة (كل صورة من صورة PNG) تمثل تسلسلًا للرسوم المتحركة. يعطي هذا تصورًا مشابهًا لملف [GIF](/ar/image/gif/). تدعم ملفات APNG صور 24 بت وشفافية 8 بت. APNG متوافق مع الإصدارات السابقة مع ملفات GIF غير المتحركة. تستخدم ملفات APNG نفس امتداد .png ويمكن فتحها بواسطة تطبيقات مثل Mozilla Firefox و Chrome مع دعم APNG وتطبيقات iMessage لنظام التشغيل iOS 10.

## نبذة تاريخية

* تم إنشاء مواصفات APNG في عام 2004 لتقديم الدعم لصور PNG المتحركة
* تم تطوير وحدات فك التشفير APNG بحجم أصغر بكثير وباستخدام الجزء الخلفي من وحدة فك ترميز PNG
* بعد المداولات المستمرة ، تمت صياغة صورة / apng من نوع MIME جديد مع الحفاظ على الامتداد كما هو .png بدلاً من .apng
* تم رفض APNG رسميًا من قبل مجموعة PNG في 20 أبريل 2007 نظرًا لتوحيدها مع صور PNG مع وجود مواصفات مختلفة في نفس الوقت

## تنسيق ملف APNG

يتم تخزين ملفات APNG كملفات ثنائية على القرص وتستخدم المواصفات الموسعة لـ PNG للصور المتحركة. الإطار الأول لملف APNG هو تدفق PNG عادي يمكن قراءته بواسطة مفكك تشفير PNG للعرض. يتبع تنسيق ملف APNG مواصفات PNG ويتم تخزين البيانات في مقاطع تسمى قطع. ومع ذلك ، قدمت APNG الأجزاء الجديدة التالية:

`` مجموعة التحكم في الرسوم المتحركة (acTL) '' - تشير إلى أن هذا الملف عبارة عن ملف PNG متحرك وليس ملف PNG عادي. يعمل كعلامة ويأتي قبل مقطع IDAT. يحتوي أيضًا على عدد الإطارات والمعلومات حول مرات تكرار الرسوم المتحركة

"مجموعة التحكم في الإطار" - تحدث في بداية كل منها ومعلومات بيانات التعريف مثل الأبعاد والموضع وتطبيق الشفافية ومعلومات الاستبدال بالإطار السابق أو التالي بمجرد انتهائها.

"مجموعة بيانات الإطار" - يخزن محتويات الإطار ويبدأ برقم تسلسلي. هذا الرقم التسلسلي له نفس بنية مقطع IDAT للصورة الافتراضية.

{{< figure src="../APNG.png" alt="صور متحركة بتنسيق PNG - تنسيق ملف APNG" >}}

APNG متوافق مع الإصدارات السابقة مع PNG حيث تم تصميم المواصفات الجانبية بطريقة تجعل من المفترض أن يتجاهل التطبيق الذي يقرأ ملف PNG ببساطة الأجزاء التي لا يفهمها. يتم استخدام المواصفات المتعلقة بعمق البت ، ونوع اللون ، والضغط ، والمرشحات ، وطرق التشابك ، ومعلومات لوح الألوان مثل تلك الخاصة بتنسيق PNG الافتراضي.

## APNG مقابل GIF

مع وجود GIF في مكانه بالفعل واستخدامه على مدار فترة زمنية طويلة ، قد تتساءل عن كيفية اختلاف APNG عن GIF. فيما يلي مجموعة من المقارنة بين APNG و GIF تعطي فكرة موجزة عن كلا تنسيقي الملف.

|| APNG | GIF |
---|---|---|
| تم النشر | 2004 | 1987 |
| عمق اللون | 24 بت | 8 بت |
| معدل الإطارات | غير محدود | 10 إطارات في الثانية |
| الشفافية | كاملة وجزئية | كاملة |
| ضغط | جيد جدا | جيد |

## مراجع

* [تنسيق ملف APNG](https://en.wikipedia.org/wiki/APNG)
* [مواصفات تنسيق PNG الرسمية](https://www.w3.org/TR/PNG/)

