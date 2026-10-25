---
title: "Rsc.Group"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De groep waartoe een resource behoort."
type: docs
weight: 300
url: /nl/net/aspose.tasks/rsc/group/
---
## Rsc.Group field

De groep waartoe een resource behoort.

```csharp
public static readonly Key<string, RscKey> Group;
```

## Voorbeelden

Toont hoe je met resource-tarieven en -groepen werkt.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Voeg een resource toe en stel enkele eigenschappen in
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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


