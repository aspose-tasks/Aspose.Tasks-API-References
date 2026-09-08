---
title: "Rsc.StandardRate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Het loonpercentage voor regulier niet-overurenwerk uitgevoerd door een resource"
type: docs
weight: 620
url: /nl/net/aspose.tasks/rsc/standardrate/
---
## Rsc.StandardRate field

Het loonpercentage voor regulier, niet‑overurenwerk uitgevoerd door een resource.

```csharp
public static readonly Key<decimal, RscKey> StandardRate;
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


