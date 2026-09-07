---
title: "Rsc.CostPerUse"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το κόστος που προκύπτει κάθε φορά που χρησιμοποιείται ένας πόρος"
type: docs
weight: 240
url: /el/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

Το κόστος που προκύπτει κάθε φορά που χρησιμοποιείται ένας πόρος.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.CostPerUse.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


