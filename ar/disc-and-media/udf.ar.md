{
  "date" : "2021-08-17",
  "keywords" :["udf file", "udf file format", "what is a udf file", "file", "udf example", "udf file extension", "extension", "format"],
  "author" : {
    "display_name" : "Muhammad Umar"
} ,
  "draft" : "false",
   "toc" : true,
  "description" :"تعرف على تنسيق ملف UDF وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات UDF وفتحها." ,
  "title" :"UDF - ملف تنسيق القرص العالمي" ,
  "linktitle" : "UDF",
  "menu" : {
    "docs" : {
      "parent" : "disc-and-media"
}
} ,
  "lastmod" : "2021-08-17"
}

## ما هو ملف UDF؟
الملف ذو الامتداد .udf هو تنسيق تصوير قرص يُستخدم عادةً لحفظ الملفات على الوسائط الضوئية ؛ يمكن استخدامها لنسخ أقراص DVD والأقراص المضغوطة والوسائط الضوئية الأخرى ؛ يخزن مجموعة من الملفات باستخدام بنية الدليل المحددة في معيار UDF ؛ يسمح بحذف الملفات وتعديلها على القرص الهدف حتى بعد كتابتها. عينت جمعية تقنية التخزين البصري نظام ملفات UDF كمعيار لتشكيل نظام ملفات مشترك لجميع الوسائط البصرية مثل الوسائط البصرية القابلة لإعادة الكتابة والوسائط للقراءة فقط.

## تنسيق ملف UDF
تنسيق ملف UDF هو نظام ملفات مفتوح البائع محايد لتخزين بيانات الكمبيوتر لمجموعة واسعة من الوسائط. تم استخدامه بشكل شائع لأقراص DVD وتنسيقات الأقراص الضوئية الأحدث. عادةً ما يتقن البرنامج نظام ملفات UDF في عملية مجمعة ويكتبها على الوسائط الضوئية في مسار واحد. ومع ذلك ، عندما يكتب الحزم إلى وسائط قابلة لإعادة الكتابة ، يسمح UDF بإنشاء الملفات وحذفها وتغييرها على القرص على غرار نظام الملفات للأغراض العامة على الوسائط القابلة للإزالة مثل محركات الأقراص المحمولة أو الأقراص المرنة.
### مواصفات UDF
يحدد معيار UDF الأشكال الثلاثة التالية لنظام الملفات:

- ** Plain Build **: هذا هو التنسيق الأصلي المدعوم في جميع مراجعات UDF. تم تقديمه في الإصدار الأول من المعيار ، ويمكن استخدام هذا التنسيق على أي نوع من الأقراص التي تتيح الوصول العشوائي للقراءة أو الكتابة ، مثل DVD + RW ، والأقراص الصلبة ، ووسائط DVD-RAM.
- ** إنشاء ضريبة القيمة المضافة **: يُستخدم خصيصًا للكتابة لوسائل الإعلام التي تكتب مرة واحدة. ضريبة القيمة المضافة هي هيكل إضافي على القرص يسمح بكتابة الحزم ؛ أي إعادة تعيين الكتل المادية عند تعديل أو حذف الملفات أو البيانات الأخرى الموجودة على القرص. بالنسبة لوسائط الكتابة مرة واحدة ، يكون القرص بأكمله افتراضيًا ، مما يجعل طبيعة الكتابة مرة واحدة شفافة للمستخدم ؛ يمكن معالجة القرص بنفس الطريقة التي يتعامل بها المرء مع قرص قابل لإعادة الكتابة.
- ** Spared (RW) build **: يُستخدم خصيصًا للكتابة على الوسائط القابلة لإعادة الكتابة. يضيف جدول Sparing إضافيًا لإدارة الأخطاء التي ستحدث في النهاية على أجزاء من القرص تمت إعادة كتابتها عدة مرات. يحفظ هذا الجدول مسار القطاعات البالية ويعيد تعيينها إلى القطاعات العاملة. لا تنطبق إدارة عيوب UDF على الأنظمة التي تنفذ بالفعل شكلاً آخر من أشكال إدارة العيوب ، مثل Mount Rainier (MRW) للأقراص الضوئية ، أو وحدة التحكم بالقرص لمحرك الأقراص الثابتة.
 




## مراجع


* [Windows Imaging Format - بواسطة Wikipedia](https://en.wikipedia.org/wiki/Windows_Imaging_Format)

