---
title: "Rsc.AvailableTo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Rsc πεδίο. Η ημερομηνία λήξης που ένας πόρος είναι διαθέσιμος για εργασία στις μονάδες που καθορίζονται για την τρέχουσα χρονική περίοδο"
type: docs
weight: 130
url: /el/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

Η ημερομηνία λήξης που ένας πόρος είναι διαθέσιμος για εργασία στις μονάδες που καθορίζονται για την τρέχουσα χρονική περίοδο.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.AvailableTo.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


