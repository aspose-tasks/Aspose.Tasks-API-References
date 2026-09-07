---
title: "Enum MonthItemType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.MonthItemType enum. Specifica l'elemento del mese per il quale è programmata una ricorrenza di eccezione"
type: docs
weight: 1050
url: /it/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

Specifica l'elemento del mese per il quale è programmata una ricorrenza di eccezione.

```csharp
public enum MonthItemType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Indica il tipo di elemento del mese non definito. |
| Day | `0` | Indica il tipo di elemento del mese Giorno. |
| Weekday | `1` | Indica il tipo di elemento del mese Giorno della settimana. |
| WeekendDay | `2` | Indica il tipo di elemento del mese Giorno del fine settimana. |
| Sunday | `3` | Indica il tipo di elemento del mese Domenica. |
| Monday | `4` | Indica il tipo di elemento del mese Lunedì. |
| Tuesday | `5` | Indica il tipo di elemento del mese Martedì. |
| Wednesday | `6` | Indica il tipo di elemento del mese Mercoledì. |
| Thursday | `7` | Indica il tipo di elemento del mese Giovedì. |
| Friday | `8` | Indica il tipo di elemento del mese Venerdì. |
| Saturday | `9` | Indica il tipo di elemento del mese Sabato. |

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


