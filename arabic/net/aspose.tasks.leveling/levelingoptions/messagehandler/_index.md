---
title: "LevelingOptions.MessageHandler"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية LevelingOptions. تحصل أو تعين رد نداء معالج الرسائل الذي يمكن استخدامه لاعتراض رسائل السجل التي ينتجها Aspose.Tasks أثناء موازنة الموارد"
type: docs
weight: 50
url: /ar/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

يحصل أو يعيّن رد نداء معالج الرسائل الذي يمكن استخدامه لاعتراض رسائل السجل التي ينتجها Aspose.Tasks أثناء موازنة الموارد.

```csharp
public IMessageHandler MessageHandler { get; set; }
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

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


