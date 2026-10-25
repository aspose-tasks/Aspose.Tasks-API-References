---
title: "Resource.Set"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Resource. Asocia la propiedad especificada al valor especificado en este contenedor"
type: docs
weight: 860
url: /es/net/aspose.tasks/resource/set/
---
## Set&lt;T&gt;(Key&lt;T, RscKey&gt;, T) {#set_1}

Mapea la propiedad especificada al valor especificado en este contenedor.

```csharp
public void Set<T>(Key<T, RscKey> key, T val)
```

| Parámetro | Descripción |
| --- | --- |
| T | el tipo del valor asignado. |
| key | la clave de propiedad especificada. [`Rsc`](../../rsc/) para obtener la clave de propiedad. |
| valor | el valor. |

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

---

## Set(Key&lt;DateTime, RscKey&gt;, DateTime) {#set}

Mapea la propiedad especificada al valor especificado en este contenedor.

```csharp
public void Set(Key<DateTime, RscKey> key, DateTime val)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | Key`2 | la clave de propiedad especificada. [`Rsc`](../../rsc/) para obtener la clave de propiedad. |
| valor | DateTime | el valor. |

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


