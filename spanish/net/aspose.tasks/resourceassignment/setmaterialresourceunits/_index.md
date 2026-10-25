---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ResourceAssignment método. Establece unidades para la asignación de un recurso material con consumo variable de material. El consumo variable de material significa que a medida que cambia la duración de la asignación, la cantidad de materiales utilizados cambia proporcionalmente"
type: docs
weight: 760
url: /es/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Establece unidades para la asignación de un recurso material con consumo de material variable. El consumo de material variable significa que, a medida que cambia la duración de la asignación, la cantidad de materiales utilizados cambia proporcionalmente.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| unidades | Double | Número de unidades acumuladas en el período de tiempo. |
| rateScaleType | RateScaleType | Período de tiempo en el que se acumula el valor de la unidad. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Si el método se llama para la asignación de un recurso no material. |

## Observaciones

Por ejemplo, para establecer '123/mes', se debe llamar a SetUnitsScaled(123D, RateScaleType.Month).

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

### Ver también

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


