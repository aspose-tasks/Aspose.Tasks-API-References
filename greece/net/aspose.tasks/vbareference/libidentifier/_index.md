---
title: "VbaReference.LibIdentifier"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "VbaReference ιδιότητα. Λαμβάνει το αναγνωριστικό της βιβλιοθήκης."
type: docs
weight: 20
url: /el/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

Λαμβάνει το αναγνωριστικό της βιβλιοθήκης.

```csharp
public string LibIdentifier { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε αναφορές VBA.

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

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


