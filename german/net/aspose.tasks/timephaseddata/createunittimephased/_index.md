---
title: TimephasedData.CreateUnitTimephased
second_title: Aspose.Tasks für .NET-API-Referenz
description: TimephasedData methode. Erstellt und initialisiert eine neue Instanz derTimephasedData Klasse für einheitenbasierte Zeitphasendaten einer Zuordnung einer Materialressource.
type: docs
weight: 30
url: /de/net/aspose.tasks/timephaseddata/createunittimephased/
---
## TimephasedData.CreateUnitTimephased method

Erstellt und initialisiert eine neue Instanz der[`TimephasedData`](../) Klasse für einheitenbasierte Zeitphasendaten einer Zuordnung einer Materialressource.

```csharp
public static TimephasedData CreateUnitTimephased(int uid, DateTime start, DateTime finish, 
    double units, TimephasedDataType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | Int32 | UID der Aufgabe. |
| start | DateTime | Startdatum-Uhrzeit. |
| finish | DateTime | Datum-Uhrzeit beenden. |
| units | Double | Anzahl der Einheiten. |
| type | TimephasedDataType | Zeitphasendatentyp. |

### Rückgabewert

Eine Instanz der[`TimephasedData`](../) Klasse für kostenbasierte Zeitphasendaten.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Wenn eine negative Anzahl von Einheiten angegeben wurde. |

### Siehe auch

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namensraum [Aspose.Tasks](../../timephaseddata/)
* Montage [Aspose.Tasks](../../../)


