---
title: "Rsc.IsCostResource"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Καθορίζει εάν ένας πόρος είναι πόρος κόστους"
type: docs
weight: 390
url: /el/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

Καθορίζει εάν ένας πόρος είναι πόρος κόστους.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.IsCostResource.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


