---
title: "Rsc.OvertimeRate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. La tarifa de pago por trabajo extra realizado por un recurso"
type: docs
weight: 510
url: /es/net/aspose.tasks/rsc/overtimerate/
---
## Rsc.OvertimeRate field

La tarifa de pago por el trabajo extra realizado por un recurso.

```csharp
public static readonly Key<decimal, RscKey> OvertimeRate;
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


