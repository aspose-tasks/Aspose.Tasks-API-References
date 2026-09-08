---
title: "Duration.ParseTimeSpan"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-methode. Parseert duurstring in het formaat PTHMS."
type: docs
weight: 130
url: /nl/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

Parseert een duurtekenreeks in het formaat "PT--H--M--S--".

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | String | de opgegeven string om te parseren. |

### Retourwaarde

retourneert een geparseerde instantie van de [`TimeSpan`](../timespan/) struct.

## Voorbeelden

Toont hoe een string om te zetten naar een tijdspan.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### Zie ook

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


