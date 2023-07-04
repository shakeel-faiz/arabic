{
  "date" : "2019-10-11",
  "keywords" :["bmp file", "bmp file format", "what is a bmp file", "file", "bmp example", "bmp file extension", "extension", "format"],
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"BMP - تنسيق ملف الصورة" ,
  "description":"تعرف على تنسيق ملف BMP وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات BMP وفتحها." ,
  "linktitle" : "BMP",
  "menu" : {
    "docs" : {
      "parent" : "image"
}
} ,
  "lastmod" : "2019-09-10"
}

# ما هو ملف BMP؟ #

الملفات ذات الامتداد .BMP تمثل ملفات الصور النقطية التي تستخدم لتخزين الصور الرقمية للصور النقطية. هذه الصور مستقلة عن محول الرسومات وتسمى أيضًا تنسيق ملف الصورة النقطية المستقلة عن الجهاز (DIB). يخدم هذا الاستقلال غرض فتح الملف على منصات متعددة مثل Microsoft Windows و Mac. يمكن لملف BMP تخزين البيانات كصور رقمية ثنائية الأبعاد بتنسيق أحادي اللون بالإضافة إلى تنسيق الألوان بأعماق ألوان مختلفة.

## مواصفات تنسيق ملف BMP ##

تعمل الصور النقطية المستقلة عن الجهاز كمساعدة في تبادل الصور النقطية بين الأجهزة والتطبيقات. نظرًا للتطور المستمر لتنسيق الملف هذا ، يمكن أن تختلف المعلومات الموجودة في الرؤوس وفقًا لإصدار Bitmap. يتكون ملف الصورة النقطية الفردي من هياكل ثابتة ومتغيرة الحجم في تسلسل معين.

يتم ترتيب الهياكل في ملف الصورة النقطية بالترتيب التالي:


| الهيكل | اختياري | الحجم | الغرض
---|---|---|---|
| رأس الملف | لا | 14 | لتخزين معلومات عامة حول ملف الصورة النقطية
| رأس DIB | لا | حجم ثابت | لتخزين معلومات مفصلة حول الصورة النقطية وتحديد تنسيق البكسل
| أقنعة بت إضافية | نعم | 12 أو 16 بايت | لتحديد تنسيق البكسل
| لوحة الألوان | شبه اختيارية | حجم متغير | لتحديد الألوان المستخدمة بواسطة بيانات الصورة النقطية
| الفجوة 1 | نعم | حجم متغير | محاذاة البنية
| صفيف البكسل | لا | حجم متغير | يتم تعريف تنسيق البكسل بواسطة رأس DIB أو أقنعة بتات إضافية.
| Gap2 | نعم | حجم متغير | محاذاة الهيكل
| ملف تعريف ألوان ICC | نعم | حجم متغير | لتعريف ملف تعريف اللون لإدارة اللون

عندما يتم تحميل صورة نقطية في الذاكرة ، فإنها تصبح بنية DIB ، يستخدمها Windows عبر واجهة برمجة تطبيقات GDI الخاصة به. رأس الملف ليس جزءًا من بنية البيانات هذه. يمكن أن يتكون اللون أيضًا من إدخالات 16 بت التي تشكل فهارس للوحة المشار إليها بشكل مجعد بدلاً من تعريفات ألوان RGB الصريحة. دعنا نلقي نظرة على بعض هذه بالتفصيل ، وخاصة الرؤوس.

### رأس ملف الصورة النقطية ###

يشبه رأس ملف الصور النقطية رؤوس الملفات الأخرى المستخدمة لتعريف الملف. نظرًا لوجود متغيرات مختلفة لتنسيق ملف BMP ، فإن أول 2 بايت من تنسيق ملف BMP هي الحرف "B" ثم الحرف "M" في ترميز ASCII. يتم تخزين جميع قيم الأعداد الصحيحة بتنسيق صغير.

| سداسي الأوفست | ديسمبر | الحجم | الغرض
---|---|---|---|
| 00 | 0 | 2 بايت | حقل الرأس المستخدم لتعريف ملف BMP و DIB هو 0x42 0x4D بالنظام الست عشري ، مثل BM في ASCII. يمكن أن تتبع القيم الممكنة. * ** BM ** - Windows 3.1x، 95، NT، ... إلخ. * ** BA ** - OS / 2 مجموعة الصور النقطية الهيكلية * ** CI ** - OS / 2 Struct رمز اللون * ** CP ** - OS / 2 const color pointer * ** IC ** - OS / 2 Struct icon * ** PT ** - OS / 2 pointer
| 02 | 2 | 4 بايت | حجم ملف BMP بالبايت
| 06 | 6 | 2 بايت | محجوز ؛ تعتمد القيمة الفعلية على التطبيق الذي ينشئ الصورة
| 08 | 8 | 2 بايت | محجوز ؛ تعتمد القيمة الفعلية على التطبيق الذي ينشئ الصورة
| 0A | 10 | 4 بايت | الإزاحة ، أي عنوان البداية ، للبايت حيث يمكن العثور على بيانات الصورة النقطية (مصفوفة البكسل).

#### رأس DIB (رأس معلومات الصورة النقطية) ####

يتم تمثيل المعلومات التفصيلية حول الصورة بواسطة هذا العنوان. بناءً على هذه المعلومات ، سيتم تحديد التطبيق الذي سيتم استخدامه لعرض الصورة على الشاشة. تحتوي كل هذه الرؤوس على حقل DWORD (32 بت) ، يحدد حجمها ، بحيث يمكن للتطبيق بسهولة تحديد الرأس المستخدم في الصورة. ويرجع ذلك أساسًا إلى حقيقة أن تنسيق بنك دبي الإسلامي قد خضع لعدة امتدادات. فيما يلي رأس DIB مع الحقول المدرجة.

#### لوحة الألوان ####

لوحة ألوان BMP هي مجموعة من الهياكل التي تحدد قيم شدة RGB لكل لون في لوحة ألوان جهاز العرض. يخزن كل بكسل في بيانات الصورة النقطية قيمة واحدة تُستخدم كفهرس في لوحة الألوان. تحدد معلومات اللون المخزنة في العنصر في هذا الفهرس لون ذلك البكسل. يختلف مدى توفر الألوان في ملف الصورة النقطية على النحو التالي:

* واحد و 4 و 8 بت - من المتوقع أن يحتوي دائمًا على لوحة ألوان
* ستة عشر و 24 و 32 بت - لا تحتوي أبدًا على لوحات ألوان
* ملفات BMP ذات ستة عشر و 32 بت - تحتوي على قيم قناع bitfields بدلاً من لوحة الألوان

#### تخزين البكسل ####

يتم تخزين وحدات البكسل النقطية على هيئة وحدات بت معبأة في صفوف حيث يتم تقريب حجم كل صف إلى مضاعفات 4 بايت (32 بت DWORD) عن طريق الحشو. لا يمكن حساب المقدار الإجمالي للبايتات المطلوبة لتخزين وحدات البكسل في الصورة مباشرةً عن طريق حساب البتات فقط. نظرًا لوجود حشوة متضمنة ، فإن تأثير تقريب حجم كل صف إلى مضاعف 4 بايت مطلوب. يجب إلحاق وحدات البايت المتروكة (ليس بالضرورة 0) بنهاية الصفوف لإحضار طول الصفوف إلى مضاعفات أربعة بايت. عند تحميل صفيف البكسل في الذاكرة ، يجب أن يبدأ كل صف من عنوان ذاكرة مضاعف لـ 4.

يتم وصف الصورة بالفعل من خلال تمثيل DWORDs 32 بت لصفيف البكسل. عادةً ما يتم تخزين وحدات البكسل "من أسفل إلى أعلى" ، بدءًا من الزاوية اليسرى السفلية ، ومن اليسار إلى اليمين ، ثم صفًا بعد صف من أسفل إلى أعلى الصورة. تنسيقات البكسل وتأثيراتها مدرجة أدناه:

* يدعم تنسيق 1 بت لكل بكسل (1 بت لكل بكسل) لونين مميزين ، (على سبيل المثال: أبيض وأسود).
* يدعم تنسيق 2 بت لكل بكسل (2 بت لكل بكسل) 4 ألوان مميزة ويخزن 4 بكسل لكل 1 بايت ، ويكون أقصى بكسل في البتتين الأكثر أهمية. كل قيمة بكسل عبارة عن فهرس 2 بت في جدول يصل إلى 4 ألوان.
* يدعم تنسيق 4 بت لكل بكسل (4 بت لكل بكسل) 16 لونًا مميزًا ويخزن 2 بكسل لكل 1 بايت ، ويكون أقصى بكسل في الجزء الأكثر أهمية. كل قيمة بكسل عبارة عن فهرس من 4 بت في جدول يصل إلى 16 لونًا.
* يدعم تنسيق 8 بت لكل بكسل (8 بت لكل بكسل) 256 لونًا مميزًا ويخزن 1 بكسل لكل 1 بايت. كل بايت عبارة عن فهرس في جدول يصل إلى 256 لونًا.
* يدعم تنسيق 16 بت لكل بكسل (16 بت لكل بكسل) 65536 لونًا مميزًا ويخزن 1 بكسل لكل 2 بايت WORD. يمكن لكل WORD تحديد عينات ألفا والأحمر والأخضر والأزرق من البكسل.
* يدعم تنسيق 24 بت بكسل (24 بت لكل بوصة) 16،777،216 لونًا مميزًا ويخزن قيمة بكسل واحد لكل 3 بايت. تحدد كل قيمة بكسل عينات الأحمر والأخضر والأزرق للبكسل (8.8.8.0.0 في تدوين RGBAX). على وجه التحديد ، بالترتيب: الأزرق والأخضر والأحمر (8 بت لكل عينة).
* يدعم تنسيق 32 بت لكل بكسل (32 بت لكل بكسل) 4،294،967،296 لونًا مميزًا ويخزن 1 بكسل لكل 4 بايت DWORD. يمكن لكل DWORD تحديد عينات ألفا والأحمر والأخضر والأزرق من البكسل.

## مراجع ##

* [تنسيق Windows MetaFile](http://msdn.microsoft.com/en-us/library/cc250370.aspx)
* [تنسيق ملف BMP](https://en.wikipedia.org/wiki/BMP_file_format)
