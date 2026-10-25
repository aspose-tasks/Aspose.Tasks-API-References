---
title: "VbaProject.References"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaProject-eigenschap. Haalt een collectie van VbaReferenceCollection op"
type: docs
weight: 70
url: /nl/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

Haalt een collectie op van [`VbaReferenceCollection`](../../vbareferencecollection/)

```csharp
public VbaReferenceCollection References { get; }
```

## Voorbeelden

Toont hoe VBA-projectreferentie-informatie te lezen.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Zie ook

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


