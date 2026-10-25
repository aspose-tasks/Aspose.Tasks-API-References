---
title: "فئة LevelingResult"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Leveling.LevelingResult. تمثل نتائج تسوية الموارد."
type: docs
weight: 960
url: /ar/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

يمثل نتائج موازنة الموارد.

```csharp
public sealed class LevelingResult
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LevelingResult](levelingresult/)() | يُنشئ مثيلًا جديدًا من الفئة `LevelingResult`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | يحصل على مجموعة من المهام المتأثرة بتسوية الموارد. |

## الأمثلة

يعرض كيفية موازنة جميع موارد المشروع باستخدام الخيارات الافتراضية.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### انظر أيضًا

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


