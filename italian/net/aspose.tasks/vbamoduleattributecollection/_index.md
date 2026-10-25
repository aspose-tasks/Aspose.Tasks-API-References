---
title: "Classe VbaModuleAttributeCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.VbaModuleAttributeCollection. Rappresenta una collezione di oggetti VbaModuleAttribute"
type: docs
weight: 2830
url: /it/net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

Rappresenta una collezione di oggetti [`VbaModuleAttribute`](../vbamoduleattribute/).

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Esempi

Mostra come iterare sulla collezione di attributi del modulo VBA.

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

### Vedi anche

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


