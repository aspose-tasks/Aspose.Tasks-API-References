---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PrimaveraProjectProperties. يحصل على معرف مشروع الخط الأساسي الحالي. ينطبق على المشاريع المقروءة من ملفات Primavera XML التي تحتوي على خطوط أساسية مُصدَّرة"
type: docs
weight: 40
url: /ar/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

يحصل على معرّف المشروع الأساسي الحالي. ينطبق على المشاريع المقروءة من ملفات Primavera XML التي تحتوي على خطوط أساسية مُصدَّرة.

```csharp
public int CurrentBaselineProjectId { get; }
```

## الأمثلة

يوضح كيفية قراءة مشروع من ملف Primavera XML وفحص بيانات مشروع الخط الأساسي.

```csharp
Project project = new Project(DataDir + "BaselineProjects.xml");

Console.WriteLine("Current baseline project uid: " + project.PrimaveraProperties.CurrentBaselineProjectId);

foreach (var baselineProject in project.PrimaveraProperties.BaselineProjects)
{
    Console.WriteLine("Baseline project: uid: {0}, name: '{1}'", baselineProject.Uid, baselineProject.Name);
}

var baseline1 = project.PrimaveraProperties.BaselineProjects[1];

var task = GetTaskByActivityId(project, "A1000");
var baselineTask = GetTaskByActivityId(baseline1, "A1000");

Console.WriteLine("Task budgeted total cost: " + task.PrimaveraProperties.BudgetedTotalCost);
Console.WriteLine("Task baseline budgeted total cost: " + baselineTask.PrimaveraProperties.BudgetedTotalCost);
```

### انظر أيضًا

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


