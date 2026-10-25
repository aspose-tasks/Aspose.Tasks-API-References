---
title: "ResourceLeveler.LevelResources"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceLeveler. تقوم بتسوية المهام للموارد المحددة باستخدام خيارات التسوية المحددة."
type: docs
weight: 30
url: /ar/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

يقوم بموازنة المهام للموارد المحددة باستخدام خيارات الموازنة المحددة.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المشروع | Project | المشروع لتطبيق تسوية الموارد. |
| خيارات | LevelingOptions | الخيارات التي تحدد كيفية تسوية الموارد. |

### قيمة الإرجاع

كائن يحتوي على نتائج تسوية الموارد.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | إذا كان معامل options فارغًا. |

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


