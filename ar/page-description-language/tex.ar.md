{
  "date" : "2019-10-11",
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"تنسيق ملف TEX" ,
  "description":"تعرف على تنسيق ملف TEX وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات TEX وفتحها." ,
  "linktitle" : "TEX",
  "menu" : {
    "docs" : {
      "parent" : "page-description-language"
}
} ,
  "lastmod" : "2019-09-10"
}

## ما هو ملف TEX؟ ##

** TeX ** هي لغة تتكون من ميزات البرمجة والترميز المستخدمة في طباعة المستندات. دونالد كنوث من جامعة ستانفورد ، هو مبتكر نظام التنضيد الغني هذا. في جميع أنحاء العالم ، تعتبر TeX هي الاختيار النهائي للمؤلفين والناشرين لإنتاج مستندات فنية عالية الجودة. يقوم TeX بعمل رائع في تنسيق التعبيرات الرياضية المعقدة. بالاقتران مع آلة الطباعة الضوئية عالية الجودة ، تتنافس TeX مع النتائج الناتجة عن أفضل أنظمة التنضيد التقليدية. لذلك يعتبر من أرقى أنظمة الطباعة الرقمية.

تستند ملفات إدخال TeX إلى كود ASCII ، مما يسمح بمشاركة المخطوطات بين الكتاب ومديري النشر والنقاد. مجموعة متنوعة من بيئات الحوسبة ، وتقريبا كل منصة حديثة والعديد من المنصات القديمة تدعم TeX. علاوة على ذلك ، فإن TeX هو برنامج مجاني متاح لمجموعة واسعة من المستهلكين. تستخدم العديد من تثبيتات UNIX كلاً من UNIX troff و TeX كنظام تنسيق لأغراض مختلفة. يتم تنفيذ مهام التنضيد الأخرى بشكل كبير في شكل حزم LaTeX و ConTeXt وحزم ماكرو أخرى.

## نبذة تاريخية ##

تم تصميم وكتابة TeX بواسطة دونالد كنوث في عام 1978. قام جاي ستيل من معهد ماساتشوستس للتكنولوجيا بمراجعة مدخلات ومخرجات TeX لجعلها تعمل في ظل نظام تشغيل غير متوافق مثل نظام مشاركة الوقت (ITS). تم تطوير الإصدار الأول من TeX وفقًا لنظام التشغيل WAITS في ستانفورد بلغة البرمجة (SAIL) وتم اختباره للتشغيل على PDP-10. قدم Knuth فكرة البرمجة المتعلمة للإصدارات المتقدمة. البرمجة الملموسة هي طريقة لتوليد كود مصدر قابل للترجمة وأنظمة تنضيد (في TeX) للتوثيق المتشابك باستخدام الملف الأصلي. تسمى اللغة المستخدمة لتطوير هذه الإصدارات المتقدمة من TeX WEB ، وهي مزيج من برامج DEC PDP-10 Pascal لضمان إمكانية النقل.

تم نشر نسخة جديدة منقحة من TeX في عام 1982 وسميت TeX82. التغيير الرئيسي هو استبدال خوارزمية الواصلة الأصلية بالخوارزمية المكتوبة حديثًا بواسطة Frank Liang. لضمان إمكانية النقل عبر منصات مختلفة ، بدلاً من استخدام النقطة العائمة ، يستخدم TeX82 حساب النقطة الثابتة إلى جانب لغة برمجة حقيقية وكاملة. في عام 1989 ، تم إصدار إصدارات جديدة من TeX و Metafont. لذا فإن الإصدار 3.0 من TeX يسهل إدخالات 8 بت ، مما يسمح لـ 256 حرفًا مختلفًا في النص. بعد الإصدار 3 ، يتم الإشارة إلى التحديثات عن طريق إضافة رقم إضافي في نهاية العلامة العشرية ، على سبيل المثال ، يشار إلى الإصدار الحالي من TeX كـ 3.14159265. تم آخر تحديث لهذا الإصدار 12-1-2014.

## مدخلات TeX ##

يمكن تحضير ملف الإدخال إلى TEX باستخدام محرر نصوص باستخدام نص عادي. بخلاف معالج Word النموذجي ، لا يسمح ملف الإدخال هذا بأي أحرف تحكم غير مرئية. يمكن تضمين ملف واحد في ملف آخر ، يحتوي على تعريفات ماكرو وتعريفات مساعدة تعزز قدرات TeX. إذا كان تثبيت TeX مصحوبًا بأي ملفات ماكرو ، فإن المعلومات المحلية حول TeX توضح استخدام ملفات الماكرو. يدمج الشكل القياسي لـ TeX مزيجًا من وحدات الماكرو والتعاريف الأخرى المعروفة باسم TEX العادي.

على أساس المعرفة الدقيقة بأحجام جميع الأحرف والرموز ، فإنه يحسب التنظيم الأمثل للحروف في كل سطر وسطر في كل صفحة. في وقت معالجة المستند ، يتم إنتاج ملف .dvi ، حيث يرمز "dvi" إلى "مستقل عن الجهاز". برامج تشغيل الجهاز مطلوبة لطباعة أو معاينة المستند بامتداد dvi. في الوقت الحاضر ، يتم تجاوز إنشاء dvi بواسطة ملف pdf- TeX شائع الاستخدام. لا تتوفر معرفة مسبقة بالخطوط في تثبيت TeX ، لذلك يتم استخدام ملفات الخطوط الخارجية ، والتي تعد جزءًا من بيئة TeX المحلية للحصول على معلومات للمستند.

## نظام الطباعة ##

يمكن فهم حوالي 300 من الأوامر الأولية (الأوامر) بواسطة نظام TeX الأساسي. الأساسيات هي أوامر منخفضة المستوى ، لذلك نادرًا ما يستخدمها المستخدم العادي بشكل مباشر ويتم تنفيذ معظم الوظائف بواسطة ملفات التنسيق. ملف التنسيق هذا عبارة عن صور ذاكرة محملة مسبقًا لـ TeX والتي يتبعها تحميل مجموعات ماكرو كبيرة. التنسيق الافتراضي الأصلي للغة ، على سبيل المثال ، يضيف TeX البسيط حوالي 600 أمر.

تشير الشرطة المائلة للخلف المجمعة بأقواس متعرجة إلى بدء أوامر TeX. نظرًا لأن TeX هي لغة قائمة على الماكرو والرمز المميز ، يمكن تغيير جميع الخصائص النحوية لـ TeX تقريبًا في وقت التشغيل ، بما في ذلك السمات المعرفة من قبل المستخدم باستثناء الرموز المميزة غير القابلة للتوسيع والتي يتم تنفيذها بعد ذلك. التوسع بحد ذاته هو عمليا خالي من المتاعب. يجب أن تأتي بعض الأوامر بعد الحجج التي تساعد في شرح وظيفة الأمر. على سبيل المثال ، يوجه الأمر \ vskip TEX لتخطي الصفحة لأسفل / لأعلى متبوعة بحجة تحدد مقدار المساحة التي يجب تخطيها.

## الإصدارات ##

LaTeX هو التنسيق الأكثر استخدامًا والذي تم تطويره في الأصل بواسطة Leslie Lamport. يدمج LaTeX أنماط مستندات مختلفة للملفات والحروف والكتب والشرائح ويقدم مراجعًا وترقيمًا تلقائيًا لأقسام مختلفة وتعبيرات رياضية. AMS-TeX هو تنسيق شائع آخر طورته الجمعية الأمريكية للرياضيات.

تقدم AMS-TeX الكثير من الأوامر سهلة الاستخدام ، والتي يمكن إعادة تعريفها بواسطة المجلات لتلائم أسلوبها المحلي. يمكن لـ LaTeX الاستفادة من مزايا AMS-TeX باستخدام "حزم" AMS والتي يطلق عليها فيما بعد AMS-LaTeX. ConTeXt هو تنسيق آخر كتبه Hans Hagen يستخدم بشكل أساسي للنشر المكتبي.

يقدم برنامج TeX العديد من الميزات التي لم تكن متوفرة ، أو ذات جودة أقل ، في أنظمة التنضيد الأخرى وقت إنشائها. تعتمد بعض الميزات المبتكرة لهذه اللغة على خوارزميات مثيرة للاهتمام مشتقة من أطروحات طلاب كنوث. بينما تدمج برامج التنضيد الأخرى الآن ميزات مفيدة لـ TeX في برامجها.

## مراجع ##

* [نظام تنضيد TeX](https://en.wikipedia.org/wiki/TeX)

