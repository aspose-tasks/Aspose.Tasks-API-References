---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "ICalendar-Methode. Berechnet das Enddatum und die Endzeit einer Aufgabe aus den aufgeteilten Teilen des Startdatums und der Arbeitsdauer."
type: docs
weight: 50
url: /de/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Berechnet das Enddatum und die Endzeit einer Aufgabe aus ihrem Startdatum, den Teilabschnitten und der Arbeitsdauer.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Aufgabe | Aufgabe | Die Aufgabe, für die das Enddatum berechnet werden soll. |
| Dauer | TimeSpan | Die zu berechnende Dauer. |

### Rückgabewert

Enddatum der Aufgabe für das gegebene Startdatum und die Dauer.

## Hinweise

Gibt DateTime.MinValue zurück, wenn die Aufgabe ein Zusammenfassung ist, null ist oder ihr Startdatum nicht gesetzt ist.

### Siehe auch

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


