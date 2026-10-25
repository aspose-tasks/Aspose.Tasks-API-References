---
title: "Resource.TimephasedData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-eigenschap. Haalt een instantie van de TimephasedDataCollection‑klasse op of stelt deze in voor dit object"
type: docs
weight: 740
url: /nl/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

Haalt een instantie op of stelt een instantie in van de klasse [`TimephasedDataCollection`](../../timephaseddatacollection/) voor dit object.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Opmerkingen

Lezen wordt alleen ondersteund voor XML-indeling.

## Voorbeelden

Toont hoe resource-tijdgephaseerde gegevens gelezen kunnen worden.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// itereren over tijdgephaseerde gegevens van de resource
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### Zie ook

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


