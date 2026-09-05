---
title: "ICalendar"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un'astrazione di calendario che può essere utilizzata per vari calcoli di date e durate."
type: docs
weight: 376
url: /it/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Rappresenta un'astrazione di calendario che può essere utilizzata per vari calcoli di date e durate.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Calcola la data in cui, secondo il calendario, trascorrerà la quantità specificata di tempo di lavoro. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Calcola la data in cui, secondo il calendario, trascorrerà la quantità specificata di tempo di lavoro. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Calcola l'inizio del prossimo giorno lavorativo per la data specificata. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Calcola la fine della data lavorativa precedente a partire dalla data specificata. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Restituisce la data di inizio basata sulla data di fine e sulla durata specificate. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Restituisce la data di inizio basata sulla data di fine e sulla durata specificate. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Calcola la data e l'ora di fine attività a partire dalla sua data di inizio, dalle parti suddivise e dalla durata del lavoro. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Calcola l'inizio del prossimo orario lavorativo a partire dalla data e ora specificate. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Restituisce la quantità di ore lavorative nella data specificata. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Restituisce WorkUnit - Inizio, Fine e Durata delle ore lavorative per l'intervallo data/ora specificato. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Restituisce la quantità di ore lavorative tra le date specificate. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Restituisce [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) dei tempi lavorativi per la data specificata. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Determina se il giorno specificato è un giorno lavorativo secondo il calendario. |
| [isEmpty()](#isEmpty--) | Restituisce se il calendario non ha ore lavorative definite. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Calcola la data in cui, secondo il calendario, trascorrerà la quantità specificata di tempo di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | Data di inizio. |
| work | [Duration](../../com.aspose.tasks/duration) | Durata del lavoro. |

**Returns:**
java.util.Date - Data di fine.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Calcola la data in cui, secondo il calendario, trascorrerà la quantità specificata di tempo di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | Data di inizio. |
| lavoro | double | Durata del lavoro. |

**Returns:**
java.util.Date - Data di fine.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Calcola l'inizio del prossimo giorno lavorativo per la data specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| data | java.util.Date | La data per ottenere l'inizio del prossimo giorno lavorativo. |

**Returns:**
java.util.Date - Inizio del prossimo giorno lavorativo System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Calcola la fine della data lavorativa precedente a partire dalla data specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| data | java.util.Date | La data per calcolare la fine del giorno lavorativo precedente. |

**Returns:**
java.util.Date - La fine del giorno lavorativo precedente
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Restituisce la data di inizio basata sulla data di fine e sulla durata specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fine | java.util.Date | La data di fine specificata. |
| duration | [Duration](../../com.aspose.tasks/duration) | La durata specificata. |

**Returns:**
java.util.Date - Data di inizio calcolata.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Restituisce la data di inizio basata sulla data di fine e sulla durata specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fine | java.util.Date | La data di fine specificata. |
| durata | double | La durata specificata. |

**Returns:**
java.util.Date - Data di inizio calcolata.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Calcola la data e l'ora di fine attività a partire dalla sua data di inizio, dalle parti suddivise e dalla durata del lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | L'attività per cui calcolare la data di fine. |
|  | durata | double | La durata da calcolare. |

Restituisce DateTime.MinValue se l'attività è un riepilogo, null o la sua data di inizio non è impostata. |

**Returns:**
java.util.Date - Data di fine dell'attività per la data di inizio e la durata fornite.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Calcola l'inizio del prossimo orario lavorativo a partire dalla data e ora specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| data | java.util.Date | La data e l'ora. |

**Returns:**
java.util.Date - L'inizio del tempo lavorativo più vicino.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Restituisce la quantità di ore lavorative nella data specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dt | java.util.Date | La data per ottenere le ore lavorative. |

**Returns:**
double - Ore lavorative nella data specificata.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


Restituisce WorkUnit - Inizio, Fine e Durata delle ore lavorative per l'intervallo data/ora specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | Data di inizio dell'intervallo. |
| fine | java.util.Date | Data di fine dell'intervallo. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Restituisce la quantità di ore lavorative tra le date specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | Data di inizio dell'intervallo. |
| fine | java.util.Date | Data di fine dell'intervallo. |

**Returns:**
double - Quantità di ore lavorative secondo l'istanza del calendario.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Restituisce [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) dei tempi lavorativi per la data specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dt | java.util.Date | La data per ottenere i tempi lavorativi. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Determina se il giorno specificato è un giorno lavorativo secondo il calendario.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dt | java.util.Date | La data per verificare se il giorno è lavorativo. |

**Returns:**
boolean - True se il giorno è lavorativo.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Restituisce se il calendario non ha ore lavorative definite.

**Returns:**
boolean - Vero se il calendario non ha ore lavorative definite.
