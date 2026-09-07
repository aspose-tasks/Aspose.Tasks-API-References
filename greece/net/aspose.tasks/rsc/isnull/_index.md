---
title: "Rsc.IsNull"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Καθορίζει εάν ένας πόρος είναι null."
type: docs
weight: 420
url: /el/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

Καθορίζει εάν ένας πόρος είναι null.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.IsNull.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


