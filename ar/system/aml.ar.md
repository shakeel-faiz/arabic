{
  "date" : "2022-04-12",
  "author" : {
    "display_name" : "Kashif Iqbal"
} ,
  "draft" : "false",
  "toc" : true,
  "title" :"ملف AML - ملف لغة الجهاز ACPI" ,
  "description":"تعرف على تنسيق ملف ACPI AML وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات AML وفتحها." ,
  "linktitle" : "AML",
  "menu" : {
    "docs" : {
      "identifier" : "system-aml",
      "parent" : "system"
}
} ,
  "lastmod" : "2022-04-12"
}

## ما هو ملف AML؟

ملف AML هو ملف نظام تم إنشاؤه باستخدام لغة التكوين المتقدم وواجهة الطاقة (ACPI) المستخدمة لتكوين خصائص الأجهزة. يحتوي على رمز بايت مستقل عن الجهاز يتم استخدامه لتكوين الأجهزة حتى للعمليات البسيطة مثل إيقاف تشغيل الكمبيوتر. قد تحتوي ملفات AML على تعليمات حسب الغرض الذي من أجله يتم تثبيتها على الجهاز. يتيح لك تنفيذ معايير ACPI تحسين وظائف إدارة الطاقة وواجهة قوية لتكوين أجهزة اللوحة الأم مثل اللوحات الأم P55.

## تنسيق ملف ACPI AML

يتم حفظ ملفات AML كملفات ثنائية على قرص بمحتويات مكتوبة برمز بايت. مواصفات تنسيق الملف لمعيار ACPI متاحة على [uefi](https://uefi.org/node/735). تم تصميم اللغة لتوفير الاستقرار والتوافق مع الإصدارات السابقة ، مما يتطلب إعادة كتابة أقل أو إعادة بناء مكدس التطبيق.

## مواصفات تنسيق ملف AML

يتكون ملف AML من جداول DSDT و SSDT. تتم قراءة كود بايت AML وتحليله من بداية كل من هذه الجداول. يوفر هذا معلومات حول تعريفات الأجهزة والكائنات في مساحة اسم ACPI. باستخدام هذه المعلومات ، يمكن لمترجم AML إنشاء قائمة بجميع الأجهزة المتاحة في النظام وخصائصها ووظائفها المدعومة.

### مثال رمز ASL لـ DSDT

مثال على رمز ASL لـ DSDT هو كما يلي.

```
DefinitionBlock ("test.aml", "DSDT", 1, "OEMID ", "TABLEID  ", 0x00000000)
{
    Scope (_SB)
    {
        Device (PCI0)
        {
            Name (_HID, EisaId ("PNP0A03"))
    }
}
}
```

## مراجع

* [ACPI AML](https://wiki.osdev.org/AML)
* [DSDT](https://wiki.osdev.org/DSDT)
* [SSDT](https://wiki.osdev.org/SSDT)
