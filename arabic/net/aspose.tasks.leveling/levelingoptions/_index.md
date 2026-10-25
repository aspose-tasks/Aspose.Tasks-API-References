---
title: "الفئة LevelingOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Leveling.LevelingOptions. تسمح بتحديد معلمات موازنة الموارد"
type: docs
weight: 940
url: /ar/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

يسمح بتحديد معلمات موازنة الموارد.

```csharp
public sealed class LevelingOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | ينشئ مثيلاً جديداً للفئة `LevelingOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | يحصل أو يعيّن رمزًا يمكن استخدامه لإلغاء عملية موازنة المشروع. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | يحصل أو يعيّن تاريخ انتهاء فترة الموازنة. القيمة الافتراضية هي تاريخ انتهاء المشروع. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | يحصل على الترتيب الذي يؤخر به خوارزمية الموازنة المهام التي لديها تخصيص زائد. بعد تحديد المهام التي تسبب التخصيص الزائد والمهام التي يمكن تأخيرها، يُستخدم الترتيب المحدد لتحديد أي مهمة يجب تأخيرها أولاً. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | يحصل أو يعيّن رد نداء معالج الرسائل الذي يمكن استخدامه لاعتراض رسائل السجل التي ينتجها Aspose.Tasks أثناء موازنة الموارد. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | يحصل أو يعيّن مستوى رسائل السجل التي تُصدرها Aspose.Tasks أثناء موازنة الموارد. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | يحصل أو يعيّن قائمة الموارد التي سيتم موازنتها. إذا تم تعيين null، سيتم موازنة جميع موارد المشروع. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | يحصل أو يعيّن تاريخ بدء فترة الموازنة. القيمة الافتراضية هي تاريخ بدء المشروع. |

## الأمثلة

يعرض كيفية تسوية مورد محدد، وتخصيص خيارات التسوية، وفحص رسائل خوارزمية التسوية.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


