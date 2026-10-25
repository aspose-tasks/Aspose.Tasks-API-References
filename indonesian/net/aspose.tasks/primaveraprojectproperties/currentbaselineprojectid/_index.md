---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PrimaveraProjectProperties. Mendapatkan Id dari proyek baseline saat ini. Berlaku untuk proyek yang dibaca dari file XML Primavera yang berisi baseline yang diekspor"
type: docs
weight: 40
url: /id/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Mendapatkan Id dari proyek baseline saat ini. Berlaku untuk proyek yang dibaca dari file XML Primavera yang berisi baseline yang diekspor.

```csharp
public int CurrentBaselineProjectId { get; }
```

## Contoh

Menampilkan cara membaca proyek dari file XML Primavera dan memeriksa data proyek baseline.

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

### Lihat Juga

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


