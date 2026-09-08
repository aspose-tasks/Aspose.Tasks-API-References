---
title: "Asn.RateScale"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La unidad de tiempo para la tasa de uso de la asignación de recurso material. Devuelve 0 si no está definido"
type: docs
weight: 410
url: /es/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

La unidad de tiempo para la tasa de uso de la asignación de recurso material. Devuelve 0 si no está definida.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## Ejemplos

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


