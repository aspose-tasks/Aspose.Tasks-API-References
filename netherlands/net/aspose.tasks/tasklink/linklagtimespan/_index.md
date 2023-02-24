---
title: LinkLagTimeSpan
second_title: Aspose.Tasks voor .NET API-referentie
description: Verkrijgt of stelt vertragingsduur in afhankelijk van LagFormat.
type: docs
weight: 50
url: /nl/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Verkrijgt of stelt vertragingsduur in, afhankelijk van LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | Bij het instellen van de waarde voor TaskLinks waarbij LagFormat TimeUnitType.Percent is. |

### Opmerkingen

Linkvertraging kan een procentuele waarde zijn (LagFormat is TimeUnitType.Percent). In dit geval wordt de duur berekend als een percentage van de duur van PredTask. Anders retourneert de methode de TimeSpan-waarde die de vertraging van TaskLink vertegenwoordigt.

### Zie ook

* class [TaskLink](../)
* naamruimte [Aspose.Tasks](../../tasklink/)
* montage [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->