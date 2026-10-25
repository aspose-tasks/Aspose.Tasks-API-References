---
title: "Rsc.Workgroup"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Het type van een werkgroep waartoe een resource behoort."
type: docs
weight: 700
url: /nl/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

Het type van een werkgroep waartoe een resource behoort.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Workgroup te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


