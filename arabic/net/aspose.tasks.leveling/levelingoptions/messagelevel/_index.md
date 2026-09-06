---
title: "LevelingOptions.MessageLevel"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية LevelingOptions. تحصل أو تعين مستوى رسائل السجل التي ينتجها Aspose.Tasks أثناء موازنة الموارد"
type: docs
weight: 60
url: /ar/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

يحصل أو يعيّن مستوى رسائل السجل التي تُصدرها Aspose.Tasks أثناء موازنة الموارد.

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


