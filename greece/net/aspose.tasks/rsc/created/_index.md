---
title: "Rsc.Created"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η ημερομηνία και ώρα που προστέθηκε ένας πόρος στο έργο"
type: docs
weight: 260
url: /el/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

Η ημερομηνία και ώρα που προστέθηκε ένας πόρος στο έργο.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Created.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


