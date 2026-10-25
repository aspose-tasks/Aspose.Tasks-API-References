---
title: "Rsc.MaxUnits"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El número máximo de unidades que representa la capacidad máxima para la cual un recurso está disponible para realizar cualquier tarea durante el período de tiempo actual"
type: docs
weight: 450
url: /es/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

El número máximo de unidades que representa la capacidad máxima para la cual un recurso está disponible para realizar cualquier tarea durante el período de tiempo actual.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.MaxUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


