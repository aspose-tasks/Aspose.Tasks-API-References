---
title: "Rsc.MaterialLabel"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η μονάδα μέτρησης για τον υλικό πόρο"
type: docs
weight: 440
url: /el/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

Η μονάδα μέτρησης για τον πόρο υλικού.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.MaterialLabel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


