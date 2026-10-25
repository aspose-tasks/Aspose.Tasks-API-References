---
title: "Rsc.Group"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El grupo al que pertenece un recurso"
type: docs
weight: 300
url: /es/net/aspose.tasks/rsc/group/
---
## Rsc.Group field

El grupo al que pertenece un recurso.

```csharp
public static readonly Key<string, RscKey> Group;
```

## Ejemplos

Muestra cómo trabajar con tarifas y grupos de recursos.

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
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


