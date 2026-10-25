---
title: "Rsc.PeakUnits"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. La unidad máxima de asignación para un recurso en cualquier momento para todas las tareas a las que el recurso está asignado"
type: docs
weight: 540
url: /es/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

La unidad máxima de asignación para un recurso en cualquier momento para todas las tareas a las que el recurso está asignado.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.PeakUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


