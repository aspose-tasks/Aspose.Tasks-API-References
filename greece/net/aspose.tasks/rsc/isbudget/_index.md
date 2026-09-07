---
title: "Rsc.IsBudget"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Καθορίζει εάν ένα υλικό εργασίας ή πόρος κόστους είναι πόρος προϋπολογισμού"
type: docs
weight: 380
url: /el/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

Καθορίζει εάν ένας πόρος εργασίας, υλικού ή κόστους είναι πόρος προϋπολογισμού.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.IsBudget.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


