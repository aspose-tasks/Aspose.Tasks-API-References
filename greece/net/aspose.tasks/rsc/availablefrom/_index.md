---
title: "Rsc.AvailableFrom"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Rsc πεδίο. Η ημερομηνία έναρξης που ένας πόρος είναι διαθέσιμος για εργασία στις μονάδες που καθορίζονται για την τρέχουσα χρονική περίοδο"
type: docs
weight: 120
url: /el/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

Η ημερομηνία έναρξης που ένας πόρος είναι διαθέσιμος για εργασία στις μονάδες που καθορίζονται για την τρέχουσα χρονική περίοδο.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.AvailableFrom.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


