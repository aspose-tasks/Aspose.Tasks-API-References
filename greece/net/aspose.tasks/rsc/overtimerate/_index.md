---
title: "Rsc.OvertimeRate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Ο ρυθμός αμοιβής για υπερωριακή εργασία που εκτελείται από έναν πόρο."
type: docs
weight: 510
url: /el/net/aspose.tasks/rsc/overtimerate/
---
## Rsc.OvertimeRate field

Ο ρυθμός αμοιβής για την υπερωριακή εργασία που εκτελείται από έναν πόρο.

```csharp
public static readonly Key<decimal, RscKey> OvertimeRate;
```

## Παραδείγματα

Δείχνει πώς να διαχειρίζεστε τις τιμές πόρων και τις ομάδες.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Προσθέστε πόρο και ορίστε κάποιες ιδιότητες
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


