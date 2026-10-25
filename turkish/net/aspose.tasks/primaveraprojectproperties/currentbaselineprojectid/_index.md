---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraProjectProperties özelliği. Mevcut temel projenin kimliğini (Id) alır. Dışa aktarılmış temel verileri içeren Primavera XML dosyalarından okunan projeler için geçerlidir"
type: docs
weight: 40
url: /tr/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Mevcut temel projenin kimliğini alır. Dışa aktarılmış temel verileri içeren Primavera XML dosyalarından okunan projeler için geçerlidir.

```csharp
public int CurrentBaselineProjectId { get; }
```

## Örnekler

Bir Primavera XML dosyasından proje nasıl okunur ve temel proje verileri nasıl incelenir gösterir.

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

### Ayrıca Bakınız

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


