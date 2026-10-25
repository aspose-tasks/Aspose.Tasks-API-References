---
title: "ResourceLeveler.LevelAll"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceLeveler. تقوم بتسوية المهام لجميع موارد المشروع باستخدام خيارات التسوية الافتراضية."
type: docs
weight: 20
url: /ar/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

يقوم بموازنة المهام لجميع موارد المشروع باستخدام خيارات الموازنة الافتراضية.

```csharp
public static LevelingResult LevelAll(Project project)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المشروع | Project | المشروع لتطبيق تسوية الموارد. |

### قيمة الإرجاع

كائن يحتوي على نتائج تسوية الموارد.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


