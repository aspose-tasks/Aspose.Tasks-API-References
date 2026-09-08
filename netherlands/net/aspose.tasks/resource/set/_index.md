---
title: "Resource.Set"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-methode. Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container"
type: docs
weight: 860
url: /nl/net/aspose.tasks/resource/set/
---
## Set&lt;T&gt;(Key&lt;T, RscKey&gt;, T) {#set_1}

Kent de opgegeven eigenschap toe aan de opgegeven waarde in deze container.

```csharp
public void Set<T>(Key<T, RscKey> key, T val)
```

| Parameter | Beschrijving |
| --- | --- |
| T | het type van de gekoppelde waarde. |
| key | de opgegeven eigenschapssleutel. [`Rsc`](../../rsc/) om de eigenschapssleutel op te halen. |
| waarde | de waarde. |

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

---

## Set(Key&lt;DateTime, RscKey&gt;, DateTime) {#set}

Kent de opgegeven eigenschap toe aan de opgegeven waarde in deze container.

```csharp
public void Set(Key<DateTime, RscKey> key, DateTime val)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | Key`2 | de opgegeven eigenschapssleutel. [`Rsc`](../../rsc/) om de eigenschapssleutel op te halen. |
| waarde | DateTime | de waarde. |

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


