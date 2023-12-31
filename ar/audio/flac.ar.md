---
date: 2019-12-13
keywords: flac , تنسيق ملف flac , امتداد flac , ملف flac , flac مقابل mp3
مؤلف:
  display_name: Muhammad Ahmad Chishti
draft: false
toc: true
description: "تعرف على تنسيق ملف FLAC وواجهات برمجة التطبيقات التي يمكنها إنشاء ملفات FLAC وفتحها."
title: تنسيق ملف FLAC
linktitle: FLAC
menu:
  docs:
    parent: "audio"
lastmod: 2021-28-05
---

## ما هو ملف FLAC؟

FLAC (Free Lossless Audio Codec) هو تنسيق ترميز صوتي مضغوط تم تطويره بواسطة Xiph.Org Foundation. FLAC هو تنسيق مفتوح بدون حقوق ملكية يتم حفظه بملحق .flac. عادةً ما يتم تقليل حجم الصوت الرقمي المضغوط باستخدام خوارزمية FLAC إلى 50 إلى 70 بالمائة. يمكن فك ضغط ملفات FLAC إلى نسخة مطابقة من ملفات الصوت الأصلية.

## تنسيق ملف FLAC

هذه نظرة عامة على تدفق بتات FLAC.

- ** علامة fLaC **: تتم إضافة هذه العلامة إلى بداية الدفق. يتبعه كتلة بيانات وصفية واحدة أو أكثر.
- ** مجموعات البيانات الوصفية **: يدعم FLAC 128 نوعًا من كتل البيانات الوصفية ؛ حاليا يتم تعريف ما يلي.
  - **STREAMINFO**: Contains the information about the whole stream.
  - **APPLICATION**: This is used by third-party applications for identification.
  - **PADDING**: It is used to reserve space for metadata if the metadata will be edited after encoding. When the metadata is edited, the padding is replaced by the actual metadata.
  - **SEEKTABLE**: An optional table to store seek points.
  - **VORBIS_COMMENT**: Used to store human-readable key/value pairs.
  - **CUESHEET**: Used to store cue sheet information.
  - **PICTURE**: Used to store pictures.
- ** FRAME **: تتكون البيانات الصوتية من إطار صوتي واحد أو أكثر.
  - **FRAME_HEADER**: Contains the basic information about the stream.
  - **SUBFRAME**: To decrease the complexity, individual subframes are coded separately within a frame (one frame per channel).
  - **FRAME_FOOTER**: Contains the CRC of the complete frame.

## تاريخ موجز لتنسيق ملف FLAC

بدأ Josh Coalson تطوير FLAC في عام 2000. تم إصدار الإصدار الأول من FLAC في 20 يوليو 2001. تم دمج FLAC تحت علامة Xiph.Org في 20 يناير 2003. تم نقل تطوير FLAC إلى مستودع Xiph.Org git مع تم إصدار النسخة 1.3.0 في 26 مارس 2013.

## تكوين مشروع FLAC

يتكون مشروع FLAC مما يلي:

- تنسيقات الدفق.
- شكل حاوية بسيط للتيار (FLAC).
- libFLAC: مكتبة من أجهزة التشفير المرجعية وأجهزة فك التشفير وواجهة البيانات الوصفية.
- libFLAC ++: غلاف كائني المنحى لـ libFLAC.
- flac: برنامج سطر أوامر لتشفير وفك تشفير تدفقات FLAC.
- ميتافلاك: محرر بيانات وصفية لسطر الأوامر لـ FLAC.
- ملحقات الإدخال لمشغلات الموسيقى مثل Winamp و XMMX وما إلى ذلك.
- شكل حاوية Ogg (Ogg FLAC).

## تصميم FLAC

اعتمادًا على كثافة الموسيقى وسعتها ، يمكن أن يكون حجم الملف المضغوط أقل بنسبة 80٪ من الملف الأصلي.

### التشفير المصدر ###

- يدعم فقط عينات الأعداد الصحيحة وليس الفاصلة العائمة. يمكنه التعامل مع دقة بت PCM من 4 إلى 32 بت لكل عينة ومعدل أخذ العينات من 1 هرتز إلى 65.535 هرتز. تشفير FLAC محدود بـ 24 بت لكل عينة.
- يمكن تجميع القنوات للاستفادة من الارتباطات بين القنوات لزيادة الضغط.
- تستخدم المجاميع الاختبارية CRC لتحديد الإطارات التالفة.
- لتحويل العينات الصوتية ، تستخدم FLAC التنبؤ الخطي.

### البيانات الوصفية ###

- يدعم FLAC ReplayGain (يستخدم لإدراك وتطبيع جهارة الصوت في الصوت).
- يستخدم FLAC نفس النظام المستخدم في تعليقات Vorbis لوضع العلامات.
- يستخدم libFLAC في معظم تطبيقات FLAC للتشفير / فك التشفير.
- يتم تنظيم libFLAC API في تدفقات وتدفقات يمكن البحث عنها وملفات لزيادة التجريد من تدفق بتات FLAC الأساسي.

### الضغط ###

يستخدم libFLAC مستويات ضغط من 0 إلى 8 حيث يكون 0 هو الأسرع و 8 هو أبطأ مستوى ضغط. تكون الملفات المضغوطة دائمًا بدون فقد على الرغم من أن المقايضة بين السرعة والحجم.

## FLAC مقابل MP3
MP3 عبارة عن تنسيق ضغط مع فقد يعني أنه قد يقطع جزءًا من الصوت لتقليل حجمه بعد تطبيق الضغط. وحيث أن FLAC هو تنسيق ملف غير ضياع مما يعني أنك قادر على سماع الصوت في أنقى صوره. في وقت سابق ، كانت تنسيقات الملفات غير المفقودة عبارة عن CDA أو WAV والتي لم تكن ذات مساحة فعالة مثل FLAC. سيوضح الجدول التالي المقارنة بين هذين التنسيقين لبعض المصطلحات المهمة:

| مصطلح | FLAC | MP3 |
---|---|---|
| ** جودة البيانات ** | لا يوجد أي فقد للبيانات الصوتية | قد تُفقد بعض البيانات عند ضغط بيانات الصوت |
| ** الحجم ** | حجم ملف أكبر مقارنة بالتنسيقات المفقودة. لذلك تحتاج إلى سعة تخزين أكبر | حجم ملف أصغر ، مناسب للتشغيل على أجهزة صوت مضغوطة مع مساحة تخزين صغيرة |
| ** متطلبات الأجهزة ** | بحاجة إلى معدات صوتية عالية الجودة وسعة تخزين ضخمة | يمكن حفظ مكتبات صوتية ضخمة في مساحة تخزين أصغر. مناسب للأجهزة المحمولة ، مثل مشغلات الصوت أو الهواتف المحمولة |
| ** التوزيع عبر الإنترنت ** | لا يمكن توزيعه بسهولة عبر الإنترنت بسبب الحجم الهائل للملف | حجم الملف المضغوط يجعل من السهل توزيعه عبر الإنترنت |
| ** التوافق ** | برنامج ترميز الموسيقى والاستماع الصوتي الأكثر شيوعًا والمتوافق إلى حد كبير مع كل جهاز على هذا الكوكب متوافق مع الجيل الجديد من أجهزة الكمبيوتر والهواتف وأجهزة استقبال الصوت والفيديو ومشغلات بلو راي وأجهزة البث مثل Roku أو Fire TV |

## مراجع ##

- [FLAC - ويكيبيديا](https://en.wikipedia.org/wiki/FLAC)

