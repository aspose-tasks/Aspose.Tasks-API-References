---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "ResourceAssignment-Methode. Gibt die Menge der zeitphasierten Arbeit für das angegebene Datums‑Zeitintervall zurück."
type: docs
weight: 730
url: /de/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Gibt die Menge der zeitphasierten Arbeit für das angegebene Datums‑Zeitintervall zurück.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Start | DateTime | Beginn des Datums‑Zeitintervalls. |
| Ende | DateTime | Ende des Datums‑Zeitintervalls. |
| timephasedDataType | TimephasedDataType | Typ der zu verwendenden zeitphasierten Daten. |

## Beispiele

Zeigt, wie die Arbeit einer Zuordnung für ein beliebiges Datum‑Uhrzeit‑Intervall berechnet wird.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Druckt die Arbeit der Zuordnung für jede Stunde.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### Siehe auch

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Gibt die Menge der zeitphasierten Arbeit für das angegebene Datums‑Zeitintervall zurück.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Start | DateTime | Beginn des Datums‑Zeitintervalls. |
| Ende | DateTime | Ende des Datums‑Zeitintervalls. |

### Siehe auch

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


