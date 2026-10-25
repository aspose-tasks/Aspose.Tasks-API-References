---
title: "ResourceAssignment.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment-methode. Retourneert een hashcodewaarde voor de instantie van de ResourceAssignment-klasse"
type: docs
weight: 710
url: /nl/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

Retourneert een hashcodewaarde voor de instantie van the [`ResourceAssignment`](../) klasse.

```csharp
public override int GetHashCode()
```

### Retourwaarde

retourneert een hashcodewaarde voor dit object.

## Voorbeelden

Toont hoe je een hashcode van een resource‑toewijzing krijgt.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// print de hashcodes van de toewijzing
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### Zie ook

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


