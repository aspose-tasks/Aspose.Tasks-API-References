---
title: "Rsc.ActualCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Rsc πεδίο. Τα κόστη που προκύπτουν για εργασία που έχει ήδη εκτελεστεί από πόρους στις εργασίες τους, μαζί με τυχόν άλλα καταγεγραμμένα κόστη που σχετίζονται με την εργασία"
type: docs
weight: 30
url: /el/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

Κόστη που προκύπτουν για εργασία που έχει ήδη εκτελεστεί από πόρους στις εργασίες τους, μαζί με τυχόν άλλα καταγεγραμμένα κόστη που σχετίζονται με την εργασία.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.ActualCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


