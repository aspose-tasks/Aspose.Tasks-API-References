---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ICalendar-methode. Berekent de einddatum en -tijd van de taak op basis van de gesplitste onderdelen van de startdatum en de werktijdduur."
type: docs
weight: 50
url: /nl/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Berekent de einddatum en -tijd van de taak op basis van de startdatum, gesplitste delen en de werktijdduur.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taak | Taak | De taak waarvoor de einddatum berekend moet worden. |
| duur | TimeSpan | De te berekenen duur. |

### Retourwaarde

Einddatum van de taak voor de gegeven startdatum en duur.

## Opmerkingen

Retourneert DateTime.MinValue als de taak een samenvatting is, null, of als de startdatum niet is ingesteld.

### Zie ook

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


