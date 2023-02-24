---
title: TimephasedData.CreateCostTimephased
second_title: Aspose.Tasks für .NET-API-Referenz
description: TimephasedData methode. Erstellt und initialisiert eine neue Instanz derTimephasedData Klasse für kostenbasierte Zeitphasendaten.
type: docs
weight: 20
url: /de/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## TimephasedData.CreateCostTimephased method

Erstellt und initialisiert eine neue Instanz der[`TimephasedData`](../) Klasse für kostenbasierte Zeitphasendaten.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | Int32 | UID der Aufgabe. |
| start | DateTime | Startdatum-Uhrzeit. |
| finish | DateTime | Datum-Uhrzeit beenden. |
| value | Double | Kostenwert. |
| timeUnit | TimeUnitType | Typ der Zeiteinheit. |
| type | TimephasedDataType | Zeitphasendatentyp. |

### Rückgabewert

Eine Instanz der[`TimephasedData`](../) Klasse für kostenbasierte Zeitphasendaten.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Wenn ein negativer Kostenwert angegeben wurde. |

### Siehe auch

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* namensraum [Aspose.Tasks](../../timephaseddata/)
* Montage [Aspose.Tasks](../../../)


