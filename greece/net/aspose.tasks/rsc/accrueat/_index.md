---
title: "Rsc.AccrueAt"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Καθορίζει πώς και πότε τα τυπικά και υπερωριακά κόστη του πόρου θα χρεωθούν ή θα συσσωρευτούν στο κόστος μιας εργασίας"
type: docs
weight: 10
url: /el/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

Καθορίζει πώς και πότε τα τυπικά και υπερωριακά κόστη πόρων θα χρεωθούν ή θα συσσωρευτούν στο κόστος μιας εργασίας.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.AccrueAt.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


