{
  "date" : "2021-05-25",
  "keywords" :["DML" , "ملف DML" , "تنسيق ملف DML" , "نوع ملف DML" , "ملف" , "النوع" , "ما هو ملف DML"] ,
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"DML - DynaScript HTML File" ,
  "description":"تعرف على تنسيق ملف DML وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات DML وفتحها." ,
  "linktitle" : "DML",
  "menu" : {
    "docs" : {
      "parent" : "web"
}
} ,
  "lastmod" : "2021-05-25"
}

## ما هو ملف DML؟

الملف بامتداد .dml هو ملف شفرة لصفحة نص برمجي على الويب تم إنشاؤه باستخدام DyanScript. DynaScript هي لغة برمجة نصية ديناميكية [HTML](/ar/web/html/) متوافقة مع ECMAScript وتوفر معظم الميزات نفسها مثل لغة البرمجة النصية الأخرى. إنه مشابه لرمز ColdFusion ورمز Microsoft Active Server Pages (ASP). يمكن فتح ملفات DML وعرضها في متصفحات الويب القياسية المشابهة لصفحات HTML الأخرى.

## تنسيق ملف DML

يتم إنشاء ملفات DML بتنسيق ملف نص عادي ويمكن فتحها باستخدام محرر نصوص لعرض الكود. يمكن استخدام كتابة التعليمات البرمجية باستخدام لغة برمجة DML لإنشاء HTML ديناميكيًا على صفحات DML المستضافة من جانب الخادم. يتم إنشاء DynaScripts من عناصر اللغة التالية:


* علامة البرنامج النصي - يتم تضمينها في المستندات كتعليقات HTML. يتم تمييز تعليق HTML بواسطة \ <!-- tag.
* Literals - هذه قيم ثابتة في ملفات DynaScript. تتضمن أمثلة هذه الأعداد الصحيحة مثل 123 ، 0x3F ، 0123 ، أرقام الفاصلة العائمة مثل 456.789 ، 3.2e-8 ، منطقية مثل صواب أو خطأ ، وسلسلة مثل "المطر في إسبانيا"
* المتغيرات - لا يلزم تعريف متغيرات DynaScript أو تعيينها إلى نوع بيانات ثابت. يجب أن يكون للمتغير قيمة قبل استخدامه في التعبير ؛ وإلا يتم إنشاء تحذير وقت التشغيل.
* التعبيرات - هي مجموعات من المتغيرات والقيم الحرفية والعوامل والتعبيرات الأخرى. الجانب الأيمن من بيان الإسناد هو تعبير.
* عوامل التشغيل - تعمل على واحد أو أكثر من التعبيرات تسمى المعاملات. يمكن أن تكون هذه إما ثلاثية أو ثنائية أو أحادية: تعمل العوامل الثلاثية على ثلاثة تعبيرات ، وتعمل العوامل الثنائية على تعبيرين ، وتعمل العوامل الأحادية على تعبير واحد.
* البيانات - تتدفق هذه البرامج النصية وتعالج الكائنات والبرمجة العامة. بشكل عام ، تتبع هذه العبارات قواعد بناء جملة C و Java القياسية. الأمثلة هي if-else ، و do-while loops ، و switch ، و break ، و continue ، وما إلى ذلك ، مثل أي لغة برمجة نصية أخرى.
* الوظائف - تسمح لك الوظائف ، مثل أي لغة برمجة نصية أخرى ، بتغليف مجموعة من الإرشادات مرة واحدة في المستند كوظيفة ، ثم استخدامها عدة مرات في المستند (عن طريق استدعاء الوظيفة). DynaScript يدعم أيضًا الوظائف.
* الكائنات - DynaScript هو كائن موجه ويدعم "الكائنات" والمفاهيم الأساسية الموجهة للكائنات مثل التغليف وتعدد الأشكال والوراثة.

