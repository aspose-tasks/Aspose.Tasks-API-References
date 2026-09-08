---
title: "Resource.Get"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource methode. Retourneert de waarde waaraan de eigenschap is toegewezen in deze container"
type: docs
weight: 830
url: /nl/net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

Retourneert de waarde waaraan de eigenschap in deze container is toegewezen.

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| Parameter | Beschrijving |
| --- | --- |
| T | het type van de gekoppelde waarde. |
| key | de opgegeven eigenschapssleutel. [`Rsc`](../../rsc/) om de eigenschapssleutel op te halen. |

### Retourwaarde

de waarde waaraan de eigenschap is toegewezen in deze container.

## Voorbeelden

Toont hoe je algemene resource-eigenschappen kunt lezen/schrijven.

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
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


