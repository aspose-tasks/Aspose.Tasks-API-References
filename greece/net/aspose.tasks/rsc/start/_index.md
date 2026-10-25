---
title: "Rsc.Start"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η ημερομηνία κατά την οποία ένας ανατεθειμένος πόρος προγραμματίζεται να αρχίσει να εργάζεται σε μια εργασία"
type: docs
weight: 640
url: /el/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

Η ημερομηνία κατά την οποία ένας εκχωρημένος πόρος έχει προγραμματιστεί να αρχίσει να εργάζεται σε μια εργασία.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Start.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


