{
  "date" : "2019-10-11",
  "keywords" :["ملف kmz" , "ما هو ملف kmz" , "ملف" , "مثال kmz" , "امتداد ملف kmz" , "امتداد" , "تنسيق"] ,
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"KMZ - تنسيق ملف KML مضغوط" ,
  "description":"تعرف على تنسيق ملف KMZ وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات KMZ وفتحها." ,
  "linktitle" : "KMZ",
  "menu" : {
    "docs" : {
      "parent" : "gis"
}
} ,
  "lastmod" : "2019-09-10"
}

## ما هو ملف KMZ؟

ملف KMZ (KML Zipped) هو تمثيل لملف مضغوط [KML](/ar/gis/kml/) يحتوي على معلومات جغرافية مكانية يمكن عرضها في تطبيقات GIS مثل Google Earth. يتم تمثيل المعلومات حول العلامات الموضعية في الملف على هيئة خطوط الطول والعرض بالإضافة إلى اسم مخصص. يمكن مشاركة ملف KMZ المنفرد الذي تم تجميعه مع مستخدمين آخرين بسهولة. يمكن أن تتضمن ملفات KMZ بيانات نموذج ثلاثي الأبعاد أيضًا للتمثيل الجغرافي للنموذج. يمكن فتح ملف KMZ في خرائط Google عن طريق حفظ الملف في موقع على الإنترنت ثم كتابة عنوان URL في مربع البحث في خرائط Google.

## هيكل الملف ##

تتكون محتويات ملف MKZ من ملف KML رئيسي وصفر أو أكثر من الملفات المرتبطة. يمكن استخراجه باستخدام أداة فك الضغط القياسية مثل WinZIP. يتم أيضًا ضغط تنسيق ملف KMZ إلى أرشيف بنسبة ضغط تبلغ 10: 1. يمكنك تصدير البيانات من Google Earth مثل التطبيقات مباشرة إلى تنسيق ملف KMZ. اسم ملف KML الرئيسي ** doc.kml **. أثناء حزم ملف KMZ ، يمكن إضافة أكثر من ملف KML إليه ، ولكن هذا لن يكون مفيدًا حيث يبحث برنامج Google Earth عن أول ملف KML عند فتح ملف KMZ وقراءته. يتجاهل أي ملفات KML أخرى موجودة في الأرشيف. للتأكد من قراءة ملف KML المطلوب بواسطة برنامج Google Earth ، يوصى بوضع ملف KML واحد فقط داخل ملف KMZ.

يتم وضع الصور والنماذج والأنسجة وملفات الصوت والموارد الأخرى المشار إليها في ملف doc.kml في مجلد فرعي آخر داخل المجلد الرئيسي. قد ينطوي هذا على بعض التعقيد أيضًا اعتمادًا على عدد الملفات الداعمة. يمكن أن تكون الروابط إلى هذه الموارد المكونة مرجعية نسبيًا أو عبر مراجع مطلقة.

### المراجع النسبية ###

عند وضع الموارد بجانب doc.kml الرئيسي داخل مجلد فرعي داخل المجلد الرئيسي ، يمكن أن تشير المراجع النسبية إلى هذه الملفات الداعمة كما هو موضح في المثال التالي (للأيقونة فقط).

```
<IconStyle>
  <scale>1.1</scale>
  <Icon>
    <href>files/icon_surfing.png</href>
  </Icon>
</IconStyle>
```

### المراجع المطلقة ###

يمكن الرجوع إلى الموارد بشكل مطلق أيضًا. تحتوي المراجع المطلقة على عنوان URL الكامل للملف المرتبط. عندما يتم نشر الملفات على خادم مركزي ، فإن المراجع المطلقة تجعلها تتأكد من أن هذه الملفات تظل واضحة مقارنة بالمراجع النسبية. لا يُنصح بالرجوع إلى الملف المحلي تمامًا لأن هذه الروابط ستتعطل عند نقل الملفات إلى نظام جديد. مثال على المرجع المطلق هو كما يلي:

```
<Icon>
  <href>http://maps.google.com/mapfiles/kml/pushpin/ylw-pushpin.png</href>
</Icon>
```

## أنظر أيضا ##

* [GeoJSON](/ar/gis/geojson/)

## مراجع ##

* [ملفات Google Earth و KMZ](https://developers.google.com/kml/documentation/kmzarchives#google-earth-and-kmz-archives)

