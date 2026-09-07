---
title: "Rsc.IsGeneric"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Καθορίζει αν ένας πόρος είναι γενικός ή όχι"
type: docs
weight: 410
url: /el/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

Καθορίζει εάν ένας πόρος είναι γενικός ή όχι.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.IsGeneric.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


