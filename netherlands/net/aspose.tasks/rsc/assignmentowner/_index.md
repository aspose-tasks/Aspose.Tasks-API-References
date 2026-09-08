---
title: "Rsc.AssignmentOwner"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De naam van een toewijzings-eigenaar."
type: docs
weight: 100
url: /nl/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

De naam van een toewijzings-eigenaar.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.AssignmentOwner te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


