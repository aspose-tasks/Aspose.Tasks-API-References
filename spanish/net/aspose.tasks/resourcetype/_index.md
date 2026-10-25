---
title: "Enum ResourceType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.ResourceType enum. Especifica el tipo de un recurso"
type: docs
weight: 1800
url: /es/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

Especifica el tipo de un recurso.

```csharp
public enum ResourceType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Material | `0` | Indica el tipo de recurso Material. |
| Work | `1` | Indica el tipo de recurso Trabajo. |
| Cost | `2` | Indica el tipo de recurso Costo. |

## Ejemplos

Muestra cómo trabajar con tipos de recurso.

```csharp
var project = new Project();

// agregar un recurso de trabajo
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// agregar un recurso material
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// agregar un recurso material
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// trabajar con recursos: crear tareas, asignar recursos, etc...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


