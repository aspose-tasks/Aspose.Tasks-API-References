---
title: "Κλάση VbaReferenceCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.VbaReferenceCollection κλάση. Αντιπροσωπεύει μια συλλογή αντικειμένων VbaReference"
type: docs
weight: 2880
url: /el/net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`VbaReference`](../vbareference/).

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη συλλογή αναφορών VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Δείτε επίσης

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


