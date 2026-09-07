---
title: "Rsc.IsEnterprise"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Δείχνει εάν ένας πόρος προέρχεται από την εταιρική ομάδα πόρων true ή από την τοπική ομάδα πόρων false."
type: docs
weight: 400
url: /el/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

Εμφανίζει εάν ένας πόρος προέρχεται από την εταιρική δεξαμενή πόρων (true) ή από την τοπική δεξαμενή πόρων (false).

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.IsEnterprise.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


