---
title: "Enumeración RateScaleType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.RateScaleType. Especifica el tipo de escala de tarifa"
type: docs
weight: 1650
url: /es/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

Especifica el tipo de escala de tarifa.

```csharp
public enum RateScaleType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `0` | Indica el tipo de escala de tarifa Undefined. |
| Minute | `1` | Indica el tipo de escala de tarifa Minute. |
| Hour | `2` | Indica el tipo de escala de tarifa Hour. |
| Day | `3` | Indica el tipo de escala de tarifa Day. |
| Week | `4` | Indica el tipo de escala de tarifa Week. |
| Month | `5` | Indica el tipo de escala de tarifa Month. |
| Quarter | `6` | Indica el tipo de escala de tarifa Quarter. |
| Year | `7` | Indica el tipo de escala de tarifa Year. |

## Ejemplos

Muestra cómo establecer el consumo variable de material (p. ej., '10/day' o '1/week') para una asignación de un recurso material.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Supongamos que queremos establecer el consumo de material '1/week'.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

Muestra cómo trabajar con la escala de tarifa de la asignación cuando queremos establecer un consumo variable de material (p. ej., '10/day' o '1/week') para una asignación de un recurso material.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Supongamos que queremos establecer el consumo de material '1/week'.
// Debemos establecer la tarifa horaria en la propiedad Units, por lo que dividimos 1D entre las horas por semana.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// Tenga en cuenta que a partir de la versión 24.4, esto puede hacerse llamando a un método:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// Solo las asignaciones de recursos materiales pueden tener un valor de escala de tarifa distinto de cero.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


