---
title: "Rsc.Finish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Rsc πεδίο. Η ημερομηνία κατά την οποία ένας πόρος προγραμματίζεται να ολοκληρώσει την εργασία σε όλες τις ανατεθειμένες εργασίες"
type: docs
weight: 290
url: /el/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

Η ημερομηνία που ένας πόρος έχει προγραμματιστεί να ολοκληρώσει την εργασία σε όλες τις ανατεθειμένες εργασίες.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Finish.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


