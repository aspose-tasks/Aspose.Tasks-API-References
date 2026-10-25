---
title: "PrimaveraProjectProperties.BaselineProjects"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PrimaveraProjectProperties. Obtiene una matriz de proyectos de línea base del proyecto actual. Es aplicable a proyectos leídos de archivos XML de Primavera que contienen líneas base exportadas"
type: docs
weight: 10
url: /es/net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

Obtiene una matriz de proyectos de línea base del proyecto actual. Es aplicable a proyectos leídos de archivos XML de Primavera que contienen líneas base exportadas.

```csharp
public Project[] BaselineProjects { get; }
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

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


