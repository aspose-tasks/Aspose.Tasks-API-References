---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskLink-eigenschap. Haalt de vertragingstijd op of stelt deze in, afhankelijk van LagFormat"
type: docs
weight: 50
url: /nl/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Haalt een waarde op of stelt deze in voor de duur van de vertraging, afhankelijk van LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentException | Bij het proberen de waarde in te stellen voor TaskLinks waarbij LagFormat TimeUnitType.Percent is. |

## Opmerkingen

Linkvertraging kan een percentagewaarde zijn (LagFormat is TimeUnitType.Percent). In dit geval wordt de duur berekend als een percentage van de duur van PredTask. Anders retourneert de methode een TimeSpan-waarde die de vertraging van TaskLink weergeeft.

### Zie ook

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


