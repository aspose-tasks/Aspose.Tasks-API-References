---
title: "Rsc.CostCenter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Υποδεικνύει σε ποιο κέντρο κόστους πρέπει να χρεωθούν τα κόστη που συσσωρεύονται από τον πόρο"
type: docs
weight: 230
url: /el/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

Δηλώνει σε ποιο κέντρο κόστους πρέπει να χρεωθούν τα κόστη που συσσωρεύονται από τον πόρο.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.CostCenter.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


