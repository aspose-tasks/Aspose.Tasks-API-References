---
title: "Notities"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "De tekstnotities die aan een toewijzing zijn gekoppeld."
type: docs
weight: 350
url: /nl/net/aspose.tasks/asn/notes/
---
## Asn.Notes field

De tekstnotities die aan een toewijzing zijn gekoppeld.

```csharp
public static readonly Key<string, AsnKey> Notes;
```

### Voorbeelden

Toont hoe resource-toewijzingsnotities op te halen/instellen.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// resource-toewijzing maken
var assn = project.ResourceAssignments.Add(task, rsc);

// resource-toewijzingsnotities instellen 
assn.Set(Asn.Notes, "Newly added assignment");

Console.WriteLine("Notes: " + assn.Get(Asn.Notes));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [AsnKey](../../asnkey)
* class [Asn](../../asn)
* namespace [Aspose.Tasks](../../asn)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
