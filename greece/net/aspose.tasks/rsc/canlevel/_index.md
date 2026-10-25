---
title: "Rsc.CanLevel"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Καθορίζει εάν μπορεί να γίνει εξισορρόπηση πόρων σε έναν πόρο"
type: docs
weight: 200
url: /el/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

Καθορίζει εάν μπορεί να γίνει εξισορρόπηση πόρων σε έναν πόρο.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.CanLevel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


