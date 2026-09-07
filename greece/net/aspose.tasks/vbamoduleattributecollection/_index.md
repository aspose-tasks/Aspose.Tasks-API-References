---
title: "Κλάση VbaModuleAttributeCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.VbaModuleAttributeCollection. Αντιπροσωπεύει μια συλλογή από αντικείμενα VbaModuleAttribute"
type: docs
weight: 2830
url: /el/net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

Αντιπροσωπεύει μια συλλογή από αντικείμενα [`VbaModuleAttribute`](../vbamoduleattribute/).

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Παραδείγματα

Δείχνει πώς να επαναλάβετε τη συλλογή χαρακτηριστικών του μονάδας VBA.

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

### Δείτε επίσης

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


