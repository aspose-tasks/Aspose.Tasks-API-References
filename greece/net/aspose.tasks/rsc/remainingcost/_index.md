---
title: "Rsc.RemainingCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το υπόλοιπο προγραμματισμένο έξοδο που θα προκύψει κατά την ολοκλήρωση της υπόλοιπης προγραμματισμένης εργασίας"
type: docs
weight: 580
url: /el/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

Το υπόλοιπο προγραμματισμένο έξοδο που θα προκύψει κατά την ολοκλήρωση της υπόλοιπης προγραμματισμένης εργασίας.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.RemainingCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


