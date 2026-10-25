---
title: "Rsc.MaxUnits"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Ο μέγιστος αριθμός μονάδων που αντιπροσωπεύει τη μέγιστη χωρητικότητα για την οποία ένας πόρος είναι διαθέσιμος να εκτελέσει οποιεσδήποτε εργασίες κατά τη διάρκεια της τρέχουσας περιόδου"
type: docs
weight: 450
url: /el/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

Ο μέγιστος αριθμός μονάδων που αντιπροσωπεύει τη μέγιστη χωρητικότητα για την οποία ένας πόρος είναι διαθέσιμος να εκτελέσει οποιεσδήποτε εργασίες κατά τη διάρκεια της τρέχουσας περιόδου.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.MaxUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


