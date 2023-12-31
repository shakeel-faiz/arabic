{
  "date" : "2019-10-11",
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"MBOX - ملف صندوق البريد الإلكتروني" ,
  "description":"تعرف على تنسيق ملف MBOX وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات MBOX وفتحها." ,
  "linktitle" : "MBOX",
  "menu" : {
    "docs" : {
      "parent" : "email"
}
} ,
  "lastmod" : "2019-09-10"
}

## ما هو ملف MBOX؟

تنسيق ملف MBox هو مصطلح عام يمثل حاوية لتجميع رسائل البريد الإلكتروني. يتم تخزين الرسائل داخل الحاوية مع مرفقاتها. يتم حفظ الرسائل من المجلد بأكمله في ملف قاعدة بيانات واحد ويتم إلحاق الرسائل الجديدة بنهاية الملف. توفر العديد من التطبيقات وواجهة برمجة التطبيقات دعمًا لتنسيق ملف MBox مثل Apple Mail و Mozilla Thunderbird.

## تنسيق ملف MBOX ##

ظل تنسيق ملف MBox غير قياسي لفترة طويلة جدًا حتى عام 2005 عندما تم توحيد التطبيق / mbox كـ [RFC 4155.](https://tools.ietf.org/rfc/rfc4155.txt) رسائل بتنسيق RFC 2822 ، متسلسلة داخل تنسيق ملف MBox واحدًا تلو الآخر. تبدأ كل رسالة بسطر فاصل يحدد مرسل الرسالة ، ويحدد أيضًا التاريخ والوقت اللذين تم فيهما استلام الرسالة من قبل المستلم النهائي (إما نظام الخطوة الأخيرة في مسار النقل ، أو النظام الذي يعمل كمستلم mailstore). يتم عادةً إنهاء كل رسالة بسطر فارغ. عادة ما يتم التعرف على نهاية قاعدة البيانات إما من خلال عدم وجود أي بيانات إضافية ، أو من خلال وجود علامة صريحة لنهاية الملف.

## قراءة رسالة من ملف MBox ##

يقوم القارئ بمسح ملف mbox بحثًا عن From_ الأسطر. أي من _ سطر يمثل بداية الرسالة. يجب ألا يحاول القارئ الاستفادة من حقيقة أن كل سطر من _ (بعد بداية الملف) سطر فارغ. بمجرد أن يعثر القارئ على رسالة ، فإنه يستخرج (ربما تالفًا) مرسل المغلف وتاريخ التسليم خارج السطر From_. ثم يقرأ حتى السطر __ التالي أو نهاية الملف ، أيهما يأتي أولاً. إنه يزيل السطر الفارغ الأخير ويحذف الاقتباس من> من _ الأسطر و >> من _ الخطوط وما إلى ذلك. والنتيجة هي رسالة RFC 822.

## اعتبارات الترميز ##

يمكن أن تتداخل محتويات ملف MBox بشكل لا رجعة فيه عندما تحتوي رسالة بريد إلكتروني مستلمة على ملف Mbox كمرفق ويتم حفظها في ملف Mbox آخر. لتجنب ذلك ، يجب أن تقوم أنظمة المراسلة بتشفير قاعدة بيانات mbox مع ترميز نقل غير شفاف (مثل BASE64 أو Quoted-Printable) كلما تم نقل مثل هذا الكائن عبر بروتوكولات المراسلة. يجب أن يكون المنفذون أيضًا على استعداد لتشفير بيانات mbox محليًا في حالة تلقي بيانات غير متوافقة.

## مراجع ##

* [MBox - RFC4155](https://tools.ietf.org/rfc/rfc4155.txt)
* [Mbox - Wikipedia](https://en.wikipedia.org/wiki/Mbox)

