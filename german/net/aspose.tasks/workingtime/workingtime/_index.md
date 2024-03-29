---
title: WorkingTime.WorkingTime
second_title: Aspose.Tasks für .NET-API-Referenz
description: WorkingTime constructeur. Initialisiert eine neue Instanz vonWorkingTime Klasse mit einem Intervall mit den angegebenen Start und Endzeiten.
type: docs
weight: 10
url: /de/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Initialisiert eine neue Instanz von[`WorkingTime`](../) Klasse mit einem Intervall mit den angegebenen Start- und Endzeiten.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fromTime | DateTime | Startzeit des Intervalls |
| toTime | DateTime | Endzeit des Intervalls |

### Siehe auch

* class [WorkingTime](../)
* namensraum [Aspose.Tasks](../../workingtime/)
* Montage [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Initialisiert eine neue Instanz von[`WorkingTime`](../) Klasse mit einem Intervallelement mit den angegebenen Start- und Endzeiten.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fromTime | TimeSpan | Startzeit des Intervalls dargestellt durchTimeSpan Struktur. |
| toTime | TimeSpan | Endzeit des Intervalls dargestellt durchTimeSpan Struktur. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Wenn toTime kleiner als gleich toTime argument ist oder wenn das Intervall zwischen fromTime und toTime größer als 24 Stunden ist. |

### Beispiele

Die Überladung von WorkingTime ctor kann verwendet werden, um den Beginn und das Ende des Intervalls mit TimeSpans: zu initialisieren.

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Siehe auch

* class [WorkingTime](../)
* namensraum [Aspose.Tasks](../../workingtime/)
* Montage [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Initialisiert eine neue Instanz von[`WorkingTime`](../) Klasse mit einem Intervallelement mit den angegebenen Start- und Endzeiten.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fromHours | Int32 | Startzeit des Intervalls, dargestellt durch ganze Stunden (0-24). |
| toHours | Int32 | Die Endzeit des Intervalls, dargestellt durch die ganze Zahl der Stunden (0–24). |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Wenn toTime kleiner als gleich toTime argument ist oder wenn das Intervall zwischen fromTime und toTime größer als 24 Stunden ist. |

### Beispiele

Die Überladung von WorkingTime ctor kann verwendet werden, um den Beginn und das Ende des Intervalls mit ganzen Stunden zu initialisieren:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

### Siehe auch

* class [WorkingTime](../)
* namensraum [Aspose.Tasks](../../workingtime/)
* Montage [Aspose.Tasks](../../../)


