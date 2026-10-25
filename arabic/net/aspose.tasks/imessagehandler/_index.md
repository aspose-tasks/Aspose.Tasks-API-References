---
title: "الواجهة IMessageHandler"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الواجهة Aspose.Tasks.IMessageHandler. تمثل رد نداء لنتائج تسوية الموارد"
type: docs
weight: 880
url: /ar/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

يمثل رد نداء لنتائج تسوية الموارد.

```csharp
public interface IMessageHandler
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | تستدعي Aspose.Tasks هذه الطريقة عند إخراج رسالة. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


