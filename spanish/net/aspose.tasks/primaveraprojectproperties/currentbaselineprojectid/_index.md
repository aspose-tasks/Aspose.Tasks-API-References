---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "PrimaveraProjectProperties propiedad. Obtiene el Id del proyecto de línea base actual. Es aplicable a proyectos leídos de archivos XML de Primavera que contienen líneas base exportadas"
type: docs
weight: 40
url: /es/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Obtiene el Id del proyecto de línea base actual. Es aplicable a proyectos leídos de archivos XML de Primavera que contienen líneas base exportadas.

```csharp
public int CurrentBaselineProjectId { get; }
```

## Ejemplos

Muestra cómo leer un proyecto de un archivo XML de Primavera y examinar los datos del proyecto de línea base.

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

### Ver también

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


