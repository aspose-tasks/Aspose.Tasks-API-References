---
title: "Rsc.Type"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Ο τύπος ενός πόρου."
type: docs
weight: 660
url: /el/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

Ο τύπος ενός πόρου.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Type.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


