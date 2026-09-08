---
title: "Resource.Get"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Resource. Devuelve el valor al que la propiedad está asignada en este contenedor"
type: docs
weight: 830
url: /es/net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

Devuelve el valor al que la propiedad está asignada en este contenedor.

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| Parámetro | Descripción |
| --- | --- |
| T | el tipo del valor asignado. |
| key | la clave de propiedad especificada. [`Rsc`](../../rsc/) para obtener la clave de propiedad. |

### Valor devuelto

el valor al que la propiedad está asignada en este contenedor.

## Ejemplos

Muestra cómo leer/escribir propiedades comunes de recursos.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Agregar recurso y establecer algunas propiedades
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


