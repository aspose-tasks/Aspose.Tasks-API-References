---
title: "ResourceLeveler.ClearLeveling"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceLeveler. تُزيل أي تأخير تسوية تم إضافته مسبقًا إلى المشروع أثناء تسوية الموارد."
type: docs
weight: 10
url: /ar/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

يمسح أي تأخير موازنة تم إضافته مسبقًا إلى المشروع أثناء موازنة الموارد.

```csharp
public static void ClearLeveling(Project project)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المشروع | Project | المشروع لإزالة التسوية. |

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

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

يمسح أي تأخير موازنة تم إضافته مسبقًا إلى المهام المحددة أثناء موازنة الموارد.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المهام | IEnumerable`1 | المجموعة القابلة للتعداد التي تحتوي على المهام التي يجب إزالة تأخير التسوية عنها. |

### انظر أيضًا

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


