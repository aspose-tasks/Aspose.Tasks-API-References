---
title: "Clase VbaModuleAttributeCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.VbaModuleAttributeCollection. Representa una colección de objetos VbaModuleAttribute"
type: docs
weight: 2830
url: /es/net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

Representa una colección de objetos [`VbaModuleAttribute`](../vbamoduleattribute/).

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Ejemplos

Muestra cómo iterar sobre la colección de atributos del módulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("Attribute Name: " + attribute.Key);
        Console.WriteLine("Attribute Value: " + attribute.Value);
    }
}
```

### Ver también

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


