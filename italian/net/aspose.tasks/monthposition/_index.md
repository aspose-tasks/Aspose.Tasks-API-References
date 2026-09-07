---
title: "Enum MonthPosition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.MonthPosition. Specifica la posizione di un elemento mensile all'interno di un mese"
type: docs
weight: 1070
url: /it/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

Specifica la posizione di un elemento del mese all'interno di un mese.

```csharp
public enum MonthPosition
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Indica la posizione mensile non definita. |
| First | `0` | Indica la prima posizione mensile. |
| Second | `1` | Indica la seconda posizione mensile. |
| Third | `2` | Indica la terza posizione mensile. |
| Fourth | `3` | Indica la posizione del quarto mese. |
| Last | `4` | Indica la posizione dell'ultimo mese. |

## Esempi

Mostra come definire un'eccezione di calendario per giorno del mese.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// crea un calendario
var calendar = project.Calendars.Add("Calendar1");

// crea un'eccezione di calendario per ogni venerdì
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// verifica che un venerdì sia eccezionale
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// aggiungi l'eccezione al calendario
calendar.Exceptions.Add(exception);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


