{
  "date" : "2019-10-11",
  "keywords" :["gbr file", "gbr file format", "what is a gbr file", "file", "gbr example", "gbr file extension", "extension", "format"],
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"تنسيق ملف GBR - تنسيق ملف جربر لثنائي الفينيل متعدد الكلور" ,
  "description":"تعرف على تنسيق ملف GBR وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات GBR وفتحها." ,
  "linktitle" : "GBR",
  "menu" : {
    "docs" : {
      "parent" : "image"
}
} ,
  "lastmod" : "2019-09-10"
}

## ما هو ملف GBR؟

الملف بامتداد gbr. هو تنسيق ملف صورة Gerber لتبادل نقل بيانات تصميم لوحة الدوائر المطبوعة (PCB). تم تطويره بواسطة Ucamco. بيانات تصميم ثنائي الفينيل متعدد الكلور هي المكون الرئيسي الذي تتطلبه صناعة التصنيع للتعامل معها. يحتوي ملف GRB على بيانات PCB مثل الطبقات النحاسية وقناع اللحام ووسيلة الإيضاح وبيانات الحفر والمسار. يمكن استخدامه لنقل البيانات مثل خصائص تصنيع ثنائي الفينيل متعدد الكلور بما في ذلك السماكة أو النهاية بتنسيق قياسي. تنتج جميع أنظمة تصميم ثنائي الفينيل متعدد الكلور ملفات جربر التي يمكن معالجتها بواسطة أنظمة تصنيع ثنائي الفينيل متعدد الكلور. أصبحت ملفات GBR الآن المعيار الفعلي لنقل بيانات تصميم لوحات الدوائر المطبوعة (PCB). قدمت Ucamco [عارضًا مجانيًا عبر الإنترنت](https://gerber-viewer.ucamco.com/) لفتح وعرض تنسيقات ملفات GBR.

## تنسيق ملف GBR

GBR هو تنسيق UTF-8 يمكن للبشر قراءته ويتكون من 27 أمرًا فقط. نظرًا لقائمة الأوامر القصيرة هذه وضغطها ، من السهل تصحيح أخطاء GBR. جربر في جوهره هو تنسيق متجه مفتوح للصور الثنائية ثنائية الأبعاد. يتم نقل المعلومات الوصفية مع الصور عبر السمات. يحدد ملف GRB واحد صورة واحدة ولا يتطلب أي ملفات مصاحبة أو معلمات خارجية ليتم تفسيرها. صورة واحدة تحتاج ملف واحد فقط. يستخدم أحرف ASCII ذات 7 بت لجميع الأوامر والأسماء المحددة في المواصفات القابلة للطباعة. يغطي هذا بشكل كامل توليد الصور بالكامل.

### مثال على ملف GBR

فيما يلي مثال على ملف جربر الذي ينشئ دائرة قطرها 1.5 مم تتمحور حول الأصل. يوجد أمر واحد في كل سطر.

```
%FSLAX26Y26*%
%MOMM*%
%ADD   100C,1.5*%
D100* X0Y0D03*
M02*
```

## مراجع

* [تنسيق جربر](https://www.ucamco.com/en/gerber)

