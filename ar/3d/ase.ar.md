{
  "date" : "2021-01-22",
  "keywords" :["ASE" , "ملف" , "تنسيق" , "نوع الملف" , "امتداد" , "ما هو ملف ASE؟" ] ,
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "description":"تعرف على تنسيق ملف ASE وواجهات برمجة التطبيقات التي يمكنها فتح ملفات ASE وإنشاؤها." ,
  "title" :"ASE - ملف تصدير مشهد Autodesk ASCII" ,
  "linktitle" : "ASE",
  "menu" : {
    "docs" : {
      "parent" : "3d"
}
} ,
  "lastmod" : "2021-01-22"
}

## ما هو ملف ASE؟

الملف بامتداد .ase هو تنسيق ملف Autodesk ASCII Scene Export يمثل تمثيل ASCII لمشهد ، يحتوي على معلومات ثنائية الأبعاد أو ثلاثية الأبعاد أثناء تصدير بيانات المشهد باستخدام Autodesk. يوفر Autodesk خيارات لتضمين مكونات المشهد أثناء تصدير بيانات المشهد. يمكنك تضمين تعريف الشبكة جنبًا إلى جنب مع معلومات الرأس والوجه ، ووصف المواد ، وتحويل بيانات الرسوم المتحركة للكائنات ، وتعريف الشبكة الكامل لكل إطارات n ، وبيانات الرسوم المتحركة للكاميرات والأضواء وإعدادات المفصل IK.

## تنسيق ملف ASE - مزيد من المعلومات

ملفات ASE هي ملفات نصية مخزنة بتنسيق ASCII يمكن فتحها في أي محرر نصوص. يمكن أن يحتوي ملف ASE على الأنواع التالية من المعلومات التي يوفرها Autodesk.

### خيارات الإخراج

* "تعريف الشبكة" - يصدر تعريف كل شبكة ، بما في ذلك معلومات الرأس والوجه للكائنات الهندسية. بالإضافة إلى ذلك ، يؤدي تشغيل هذا إلى تمكين العناصر الموجودة في مربع مجموعة خيارات الشبكة ، الموضح أدناه.
* "المواد" - تشمل وصف المادة. إذا لم يتم تعيين مادة لكائن ، يتم تصدير لون الإطار السلكي الخاص بها. يتم تضمين جميع مستويات شجرة المواد ، لذلك يمكن أن ينتج عن ذلك الكثير من النص.
* "تحويل مفاتيح الرسوم المتحركة" - يشمل تحويل بيانات الرسوم المتحركة للكائنات. إذا كان الكائن عبارة عن كاميرا مستهدفة أو بقعة ضوء ، فسيشمل ذلك بيانات الرسوم المتحركة المستهدفة.
* "شبكة متحركة" - يصدر تعريف شبكة كاملة لكل عدد n من الإطارات. يتم تحديد التردد بواسطة وحدة التحكم في الإخراج ، الموضحة أدناه. تحتوي كل كتلة على نفس المعلومات المحددة في مربع مجموعة خيارات الشبكة ، الموضح أدناه. يمكن أن ينتج عن تشغيل هذا ملف ضخم ، حتى بالنسبة للمشاهد الصغيرة.
* "إعدادات الكاميرا / الإضاءة المتحركة" - لتصدير بيانات الرسوم المتحركة للكاميرات والأضواء ، مثل اللون ، والشدة ، والانخفاض ، وانحياز الخريطة ، وما إلى ذلك. يخرج كتلة كل n إطارات ، كما هو محدد بواسطة زر إخراج وحدة التحكم.
* "المفاصل الحركية العكسية" - لتصدير الإعدادات المشتركة IK في فرع التسلسل الهرمي.

### أنواع الكائنات

تتيح لك العناصر هنا تحديد فئة الكائن التي تريد تضمينها في الإخراج. يمكنك تضمين كائنات وأشكال وكاميرات وأضواء وكائنات مساعدة هندسية.

* هندسي
* الأشكال
* الكاميرات
* أضواء
* المساعدون

### خيارات الشبكة

* "Mesh Normals" - لتصدير الأعراف في الوجه والرأس. يُدرج الوجه الطبيعي أولاً ، متبوعًا بقواعد الرؤوس الثلاثة التي تدعم الوجه. يؤدي تشغيل هذا إلى ملف أكبر بكثير.
* "إحداثيات التعيين" - يصدر قائمة برؤوس الخرائط والوجوه ، وفقًا لبنية TVert و TVFace الموصوفة في 3ds Max Software Development Kit. إذا كان الكائن يستخدم تعيين الوجه ، يتم تصدير قائمة خريطة الوجه تحتوي على إحداثيات UVW لكل وجه.
* "ألوان الرأس" - لتصدير ألوان الرأس.

### إخراج تحكم

* "استخدام المفاتيح" - لتصدير قيم المفاتيح. إذا لم تستخدم وحدة التحكم المفاتيح ، فسيتم استخدام طريقة نموذج القوة. في حالة وحدات التحكم في المحولات ، لا يعمل خيار Use Keys إلا إذا كانت جميع وحدات التحكم في المحولات إما Linear / TCB أو Bezier. إذا كان أحد مسارات التحويل يستخدم نوعًا مختلفًا من وحدة التحكم ، فسيتم استخدام طريقة نموذج القوة لجميع مسارات التحويل.
* "عينات القوة" - عينات قيم وحدة التحكم بناءً على التردد المحدد في الإطارات لكل وحدة تحكم عينة.

## مراجع

* [Autodesk - Exporting to ASCII](https://help.autodesk.com/view/3DSMAX/2020/ENU/?guid=GUID-98B2388D-A3A7-4096-8E81-888A3F9D6069)

