{
  "date" : "2021-06-24",
  "keywords" :["ملف بات" , "ما هو ملف بات" , "ملف" , "مثال ملف بات" , "امتداد" , "تنسيق"] ,
  "author" : {
    "display_name" : "Muhammad Umar"
} ,
  "draft" : "false",
  "toc" : true,
  "description":"تعرف على تنسيق ملف BAT وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات BAT وفتحها." ,
  "title" :"BAT - تنسيق ملف دفعي" ,
  "linktitle" : "BAT",
  "menu" : {
    "docs" : {
      "parent" : "executable"
}
} ,
  "lastmod" : "2021-06-24"
}

## ما هو ملف BAT؟
يُعرف ملف BAT بأنه ملف دفعي يعمل مع DOS وجميع إصدارات Windows ، ضمن cmd.exe. وهو يتألف من سلسلة من أوامر الأسطر في نص عادي ليتم تنفيذها بواسطة مترجم سطر الأوامر لأداء مهام مختلفة ، مثل تشغيل أدوات الصيانة داخل Windows أو بدء تشغيل البرامج النموذجية. قد يشتمل الملف الدفعي على أي أمر يمكن أن يقبله المترجم بشكل تفاعلي ويستخدم بنية الكود التي تتيح التفريع الشرطي والتكرار الحلقي كما هو مكتوب في الملف الدفعي.
## تنسيق ملف BAT
تنسيق ملف BAT هو ببساطة برنامج نصي مدمج لأتمتة تسلسلات الأوامر التي تكون متكررة بطبيعتها. يستخدم مصطلح "الدُفعة" لمعالجة الدُفعات ، ويمكن اعتباره "تنفيذًا غير تفاعلي". لذلك قد لا يعالج ملف دفعي دفعة من بيانات متعددة. في نظام تشغيل القرص القديم (DOS) ، تم تشغيل الملف الدفعي تحت واجهة سطر الأوامر عن طريق كتابة اسم الملف والملحق .bat. كان نظام التشغيل السابق المستند إلى الواجهة الرسومية لـ Microsoft مثل Microsoft Windows يعتمد على DOS. كان على المستخدمين استخدام DOS لإجراء عمليات نموذجية مثل إصلاح Windows أو تحسينه أو إعادة تثبيته. في وقت لاحق قدمت مايكروسوفت نظام التشغيل Windows NT الذي لم يكن يعتمد على نظام التشغيل DOS. لذلك ، يمكن تشغيل الملفات الدفعية باستخدام موجه الأوامر أو ** cmd.exe ** في أنظمة تشغيل Microsoft الحديثة.
### معلمات الملف الدفعي
يدعم موجه الأوامر عددًا من المتغيرات الخاصة مثل **٪ 0 و٪ 1 إلى٪ 9 ** للإشارة إلى اسم ومسار الوظيفة الدفعية ومعلمات الاستدعاء التسعة من داخل الوظيفة الدفعية. يتم استبدال المعلمات غير الموجودة بسلسلة ذات طول صفري. على الرغم من أنه يمكن استخدامها بشكل مشابه لمتغيرات البيئة ، ولكن لا يتم حفظها في البيئة. تشير Microsoft و IBM إلى هذه المتغيرات كمعلمات بديلة ، بينما قدمت Novell و Digital Research و Caldera مصطلح متغيرات الاستبدال لها.

فيما يلي بعض أوامر الملفات الدفعية المفيدة:
| أمر | الوصف |
------|------------|
| VER | يعرض هذا الأمر الدفعي إصدار MS-DOS الذي تستخدمه. |
| ASSOC | هذا أمر دفعي يربط امتدادًا بنوع ملف (FTYPE) ، أو يعرض الاقترانات الموجودة ، أو يحذف اقترانًا. |
| قرص مضغوط | يساعد هذا الأمر الدُفعي في إجراء تغييرات على دليل مختلف ، أو يعرض الدليل الحالي. |
| CLS | هذا الأمر الدُفعي يمسح الشاشة. |
| نسخ | يتم استخدام هذا الأمر الدُفعي لنسخ الملفات من موقع إلى آخر. |
| DEL | هذا الأمر الدُفعي يحذف الملفات وليس الدلائل. |
| DIR | يسرد هذا الأمر الدُفعي محتويات الدليل. |
| التاريخ | يساعد أمر الدُفعات هذا في العثور على تاريخ النظام. |
| صدى | يعرض هذا الأمر الدُفعي الرسائل ، أو يقوم بتشغيل أو إيقاف تشغيل صدى الأوامر. |
| خروج | يتم إنهاء هذا الأمر الدُفعي من وحدة تحكم DOS. |
| MD | يقوم هذا الأمر الدُفعي بإنشاء دليل جديد في الموقع الحالي. |
| نقل | يقوم أمر الدُفعات هذا بنقل الملفات أو الدلائل بين الدلائل. |
| المسار | يعرض هذا الأمر الدُفعي أو يحدد متغير المسار. |
| وقفة | يطالب هذا الأمر الدُفعي المستخدم وينتظر إدخال سطر إدخال. |
| PROMPT | يمكن استخدام هذا الأمر الدفعي لتغيير أو إعادة تعيين موجه cmd.exe. |
| RD | يقوم أمر الدُفعات هذا بإزالة الدلائل ، ولكن يجب أن تكون الدلائل فارغة قبل إزالتها. |
| رن | يعيد تسمية الملفات والدلائل |
| REM | يتم استخدام هذا الأمر الدُفعي للملاحظات في الملفات الدفعية ، مما يمنع تنفيذ محتوى الملاحظة. |
| ابدأ | يبدأ هذا الأمر الدُفعي برنامجًا في نافذة جديدة ، أو يفتح مستندًا. |
| الوقت | يقوم هذا الأمر الدُفعي بتعيين الوقت أو عرضه. |
| النوع | يقوم هذا الأمر الدُفعي بطباعة محتوى ملف أو ملفات إلى الإخراج. |
| المجلد | يعرض هذا الأمر الدُفعي تسميات وحدة التخزين. |
| اتريب | يعرض أو يحدد سمات الملفات في الدليل الحالي |
| CHKDSK | يتحقق هذا الأمر الدُفعي من القرص بحثًا عن أية مشكلات. |
| اختيار | يوفر هذا الأمر الدُفعي قائمة بالخيارات للمستخدم. |
| CMD | يستدعي هذا الأمر الدُفعي مثيلًا آخر من موجه الأوامر. |
| كوم | يقارن هذا الأمر الدفعي ملفين بناءً على حجم الملف. |
| تحويل | يقوم هذا الأمر الدُفعي بتحويل وحدة تخزين من نظام ملفات FAT16 أو FAT32 إلى نظام ملفات NTFS. |
| طلب القيادة | يعرض هذا الأمر الدُفعي جميع برامج تشغيل الأجهزة المثبتة وخصائصها. |
| توسيع | يقوم هذا الأمر الدفعي باستخراج الملفات من ملفات الخزانة. cab المضغوطة. |
| البحث | يبحث أمر الدُفعات هذا عن سلسلة في الملفات أو الإدخال ، ويخرج سطورًا متطابقة. |
| تنسيق | يقوم أمر الدُفعات هذا بتنسيق قرص لاستخدام نظام الملفات المدعوم من Windows مثل FAT أو FAT32 أو NTFS ، وبالتالي الكتابة فوق المحتوى السابق للقرص. |
| مساعدة | يعرض هذا الأمر الدُفعي قائمة الأوامر التي يوفرها Windows. |
| IPCONFIG | يعرض هذا الأمر الدفعي تكوين Windows IP. يظهر التكوين عن طريق الاتصال واسم ذلك الاتصال. |
| LABEL | يقوم أمر الدُفعات هذا بإضافة تسمية قرص أو تعيينها أو إزالتها. |
| المزيد | يعرض هذا الأمر الدُفعي محتويات ملف أو ملفات ، شاشة واحدة في كل مرة. |
| NET | يوفر خدمات شبكة متنوعة ، حسب الأمر المستخدم. |
| بينغ | يرسل هذا الأمر الدُفعي حزم "echo" ICMP / IP عبر الشبكة إلى العنوان المحدد. |
| اغلاق | يقوم هذا الأمر الدُفعي بإيقاف تشغيل الكمبيوتر أو تسجيل خروج المستخدم الحالي. |
| الترتيب | يأخذ هذا الأمر الدُفعي المدخلات من ملف مصدر ويفرز محتوياته أبجديًا ، من A إلى Z أو Z إلى A. ويطبع الإخراج على وحدة التحكم. |
| ثانوي | يقوم الأمر الدُفعي هذا بتعيين حرف محرك أقراص إلى مجلد محلي ، أو يعرض التعيينات الحالية ، أو يزيل مهمة. |
| SYSTEMINFO | يعرض هذا الأمر الدُفعي تكوين جهاز الكمبيوتر ونظام التشغيل الخاص به. |
| TASKKILL | هذا الأمر الدُفعي ينهي مهمة واحدة أو أكثر. |
| قائمة المهام | يسرد هذا الأمر الدفعي المهام ، بما في ذلك اسم المهمة ومعرف العملية (PID). |
| XCOPY | يقوم أمر الدُفعات هذا بنسخ الملفات والدلائل بطريقة أكثر تقدمًا. |
| شجرة | يعرض هذا الأمر الدُفعي شجرة لجميع الدلائل الفرعية للدليل الحالي إلى أي مستوى من العودية أو العمق. |
| FC | يسرد هذا الأمر الدفعي الاختلافات الفعلية بين ملفين. |
| DISKPART | يعرض هذا الأمر الدفعي خصائص أقسام القرص ويقوم بتكوينها. |
| العنوان | يعيّن هذا الأمر الدفعي العنوان المعروض في نافذة وحدة التحكم. |
| مجموعة | يعرض قائمة متغيرات البيئة على النظام الحالي. |

## مثال على ملف BAT
عادةً ما يتم حفظ البرامج النصية المجمعة كملفات نصية بسيطة ؛ تحتوي على أوامر يتم تنفيذها في تسلسل. يتم حفظ هذه الملفات بامتداد .bat ؛ تم التعرف عليها وتنفيذها باستخدام برنامج ** Command Interpreter **. يتوفر هذا البرنامج أصلاً في Microsoft Windows باسم ** cmd.exe **.

إليك نموذج Batch Script الذي يحذف جميع الملفات في الدليل الحالي:
```
:: Deletes All files in the Current Directory With Prompts and Warnings
::(Hidden, System, and Read-Only Files are Not Affected)
:: @ECHO OFF
DEL . DR
```


## مراجع

* [Batch Script - Quick Guide](https://www.tutorialspoint.com/batch_script/batch_script_quick_guide.htm)
* [ملف دفعي - بواسطة Wikipewdia](https://en.wikipedia.org/wiki/Batch_file)

