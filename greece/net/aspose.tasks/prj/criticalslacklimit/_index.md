---
title: "Prj.CriticalSlackLimit"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Οι εργασίες θεωρούνται κρίσιμες από το MS Project εάν το συνολικό περιθώριο είναι μικρότερο ή ίσο με αυτόν τον αριθμό ημερών"
type: docs
weight: 140
url: /el/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

Οι εργασίες θεωρούνται κρίσιμες από το MS Project εάν η συνολική ελεύθερη ώρα είναι μικρότερη ή ίση με αυτόν τον αριθμό ημερών.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.CriticalSlackLimit.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


