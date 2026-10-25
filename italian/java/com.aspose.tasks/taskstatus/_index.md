---
title: "TaskStatus"
second_title: "Aspose.Tasks for Java API Reference"
description: "Specifica lo stato di un'attività."
type: docs
weight: 301
url: /it/java/com.aspose.tasks/taskstatus/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TaskStatus extends System.Enum
```

Specifica lo stato di un'attività.
## Campi

| Campo | Descrizione |
| --- | --- |
| [Complete](#Complete) | L'attività è completata al 100 percento. |
| [Future](#Future) | Lo stato dell'attività 'Future' viene impostato quando la data di inizio dell'attività è successiva alla data di stato. |
| [Late](#Late) | L'attività è in ritardo se la percentuale cumulativa temporizzata completata non raggiunge la mezzanotte del giorno precedente alla data di stato. |
| [OnSchedule](#OnSchedule) | L'attività è in programma se la percentuale cumulativa temporizzata completata è distribuita almeno fino al giorno precedente alla data di stato. |
| [Undefined](#Undefined) | Stato dell'attività non definito. |
### Complete {#Complete}
```
public static final int Complete
```


L'attività è completata al 100 percento.

### Future {#Future}
```
public static final int Future
```


Lo stato dell'attività 'Future' viene impostato quando la data di inizio dell'attività è successiva alla data di stato.

### Late {#Late}
```
public static final int Late
```


L'attività è in ritardo se la percentuale cumulativa temporizzata completata non raggiunge la mezzanotte del giorno precedente alla data di stato.

### OnSchedule {#OnSchedule}
```
public static final int OnSchedule
```


L'attività è in programma se la percentuale cumulativa temporizzata completata è distribuita almeno fino al giorno precedente alla data di stato.

### Undefined {#Undefined}
```
public static final int Undefined
```


Stato dell'attività non definito.

