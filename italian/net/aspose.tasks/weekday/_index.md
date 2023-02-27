---
title: Class WeekDay
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.WeekDay classe. Rappresenta un giorno della settimana che definisce i giorni regolari della settimana o i giorni di eccezione in un calendario.
type: docs
weight: 3180
url: /it/net/aspose.tasks/weekday/
---
## WeekDay class

Rappresenta un giorno della settimana che definisce i giorni regolari della settimana o i giorni di eccezione in un calendario.

```csharp
public class WeekDay
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Inizializza una nuova istanza di`WeekDay` classe. |
| [WeekDay](weekday/#constructor_1)(DayType) | Inizializza una nuova istanza di`WeekDay` classe con il tipo di giorno specificato. |
| [WeekDay](weekday/#constructor_2)(DayType, IEnumerable&lt;WorkingTime&gt;) | Inizializza una nuova istanza di`WeekDay` classe con il tipo di giorno specificato e l'elenco dei periodi di orario di lavoro. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Ottiene il tipo di un giorno. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Ottiene o imposta un valore che indica se la data o il tipo di giorno specificato funziona. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Ottiene o imposta l'inizio di un tempo di eccezione. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Ottiene o imposta la fine di un tempo di eccezione. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Ottiene WorkingTimeCollection per questa istanza WeekDay. La raccolta di orari di lavoro che definiscono il tempo lavorato nel giorno della settimana. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Crea il giorno lavorativo predefinito. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Restituisce una copia completa del giorno della settimana. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Restituisce un valore di codice hash per l'istanza di`WeekDay` classe. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Restituisce l'orario di lavoro per un giorno della settimana. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Lancia .NetDayOfWeek A[`DayType`](./daytype/) . |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Imposta i periodi di tempo predefiniti per il giorno della settimana specificato. |

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks/)
* assemblea [Aspose.Tasks](../../)


