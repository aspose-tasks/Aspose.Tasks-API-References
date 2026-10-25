---
title: "Rsc.PeakUnits"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η μέγιστη μονάδα ανάθεσης για έναν πόρο σε οποιαδήποτε χρονική στιγμή για όλες τις εργασίες στις οποίες έχει ανατεθεί ο πόρος"
type: docs
weight: 540
url: /el/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

Η μέγιστη μονάδα ανάθεσης για έναν πόρο σε οποιαδήποτε χρονική στιγμή για όλες τις εργασίες στις οποίες έχει ανατεθεί ο πόρος.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.PeakUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


