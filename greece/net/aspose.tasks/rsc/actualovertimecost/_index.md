---
title: "Rsc.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Κόστη που προέκυψαν για υπερωριακή εργασία που έχει ήδη εκτελεστεί σε εργασίες από τους ανατεθειμένους πόρους"
type: docs
weight: 40
url: /el/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

Κόστη που προκύπτουν για υπερωριακή εργασία που έχει ήδη εκτελεστεί σε εργασίες από τους εκχωρημένους πόρους.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.ActualOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


