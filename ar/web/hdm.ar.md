{
  "date" : "2022-10-12",
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"ملف HDM - ملف لغة توصيف الجهاز المحمول" ,
  "description":"تعرف على تنسيق ملف HDM وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات HDM وفتحها." ,
  "linktitle" : "HDM",
  "menu" : {
    "docs" : {
      "parent" : "web"
}
} ,
  "lastmod" : "2022-10-12"
}

## ما هو ملف HDM؟

ملف HDM هو ملف صفحة ويب لغة ترميز يتم إنشاؤه بلغة توصيف الجهاز المحمول (HDML). يحتوي على علامات ترميز مشابهة للغة [HTML](/ar/ web / html /) ، ولكنه مصمم للأجهزة الإلكترونية المحمولة مثل الهواتف الذكية وأجهزة المساعد الرقمي الشخصي. تم إرسال [مواصفات تنسيق ملف HDML](https://www.w3.org/TR/NOTE-Submission-HDML-spec.html) إلى W3C للتوحيد ولكن لا يمكن أن تصبح معيارًا. يعتمد HDM على مواصفات تنسيق الملف [HDML](/ar/ web / hdml /) المتوفرة على موقع W3.

## تنسيق ملف HDM - مزيد من المعلومات

يتكون ملف HDM من علامات تمييز يتم عرضها على موقع ويب مصمم بصريًا على الأجهزة المحمولة. يتم نسخ ملفات HDM إلى الأجهزة التي تستخدم بروتوكول HDTP (بروتوكول نقل الجهاز المحمول) بدلاً من بروتوكول HTTP المستخدم لصفحات HTML.

## عناصر ملف HDML

فيما يلي مجموعة صغيرة من العناصر التي توفر بيئة وقت التشغيل لـ HDML ويشار إليها باسم وكيل المستخدم.

| العنصر | الوصف |
---|---|
| البطاقات | هذا هو لبنة البناء الأساسية لـ HDML ، ويعرض ويسمح للمستخدم بالتفاعل مع بطاقات المعلومات. |
| الطوابق | بطاقات HDML مجمعة معًا في مجموعات. تشبه مجموعة HDML صفحة HTML حيث يتم تعريفها بواسطة URL [RFC1738] وهي وحدة المحتوى المطلوبة من الخادم وتخزينها مؤقتًا بواسطة وكيل المستخدم.
| الإجراءات | يمكن أن تكون الإجراءات من نوع PREV و SOFT1-SOFT8 و HELP. هذه هي مجردة ويتم دعمها في واجهة المستخدم بطريقة محددة وكيل المستخدم
| الأنشطة | النشاط يشبه مجموعة البطاقات ذات الصلة التي تؤدي وظيفة منطقية واحدة. قد تمتد هذه على سطح واحد أو أكثر. تم بناء نموذج حالة تنقل وحالة HDML حول الأنشطة
| التنقل المستند إلى المحفوظات | يحتفظ وكيل المستخدم بمحفوظات البطاقات المعروضة للمستخدم. تتم إضافة كل بطاقة يتم الوصول إليها إلى سجل البطاقة. يسمح وكيل المستخدم للمستخدم بالانتقال بسهولة إلى البطاقة السابقة في السجل. |

## مراجع

* [HDML - ويكيبيديا](https://en.wikipedia.org/wiki/Handheld_Device_Markup_Language)
* [مواصفات HDML - مدارس W3](https://www.w3.org/TR/NOTE-Submission-HDML-spec.html)
