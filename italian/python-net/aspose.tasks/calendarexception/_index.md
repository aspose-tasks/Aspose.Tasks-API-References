---
title: "CalendarException"
second_title: "Riferimento API di Aspose.Tasks per Python via .NET"
description: 
type: docs
weight: 160
url: /it/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

Rappresenta periodi di tempo eccezionali in un calendario.

Il tipo CalendarException espone i seguenti membri:
## Costruttori
| Nome | Descrizione |
| :- | :- |
| CalendarException() | Inizializza una nuova istanza della classe [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/). |
## Proprietà
| Nome | Descrizione |
| :- | :- |
| entered_by_occurrences | Ottiene o imposta un valore che indica se l'intervallo di ricorrenza è definito inserendo un numero di occorrenze.<br/>            False specifica che l'intervallo di ricorrenza è definito inserendo una data di fine. |
| from_date | Ottiene o imposta l'inizio del periodo di eccezione. |
| to_date | Ottiene o imposta la fine del periodo di eccezione. |
| occurrences | Ottiene o imposta il numero di occorrenze per le quali l'eccezione del calendario è valida. |
| name | Ottiene o imposta il nome dell'eccezione. |
| tipo | Ottiene o imposta il tipo di eccezione. |
| period | Ottiene o imposta il periodo di ricorrenza per l'eccezione. |
| days_of_week | Ottiene la DayTypeCollection per questo oggetto.<br/>            I giorni della settimana in cui l'eccezione è valida. |
| month_item | Ottiene o imposta l'elemento del mese per il quale è programmata una ricorrenza di eccezione. |
| month_position | Ottiene o imposta la posizione di un elemento del mese all'interno di un mese. |
| month | Ottiene o imposta il mese per il quale è programmata una ricorrenza di eccezione. |
| month_day | Ottiene o imposta il giorno del mese in cui è programmata una ricorrenza di eccezione. |
| day_working | Ottiene o imposta un valore che indica se la data o il tipo di giorno specificati sono lavorativi. |
| working_times | Ottiene o imposta l'oggetto WorkingTimeCollection.<br/>            La collezione di orari di lavoro che definisce il tempo lavorato nei giorni feriali. |
| parent_calendar | Restituisce il calendario padre per questo oggetto. |
## Methods
| Nome | Descrizione |
| :- | :- |
| delete() | Elimina l'istanza Exception dal calendario genitore oggetto CalendarExceptionCollection. |
| check_exception(dt) | Restituisce true se l'istanza specificata della struttura datetime è il giorno di eccezione. |
| get_working_time() | Restituisce il tempo di lavoro per un'eccezione del calendario. |
| get_exception_dates() | Restituisce le date in cui l'eccezione del calendario è applicabile. |

### Vedi anche

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

