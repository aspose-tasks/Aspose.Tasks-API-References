---
title: "Rsc.CostVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η διαφορά μεταξύ του αρχικού κόστους και του συνολικού κόστους για έναν πόρο"
type: docs
weight: 250
url: /el/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

Η διαφορά μεταξύ του κόστους βάσης και του συνολικού κόστους για έναν πόρο.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.CostVariance.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


