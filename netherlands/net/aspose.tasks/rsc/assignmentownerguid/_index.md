---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De GUID van een toewijzings-eigenaar."
type: docs
weight: 110
url: /nl/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

De GUID van een toewijzings-eigenaar.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.AssignmentOwnerGuid te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


