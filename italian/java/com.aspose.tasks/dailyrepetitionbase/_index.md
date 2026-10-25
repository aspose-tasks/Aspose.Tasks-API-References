---
title: "DailyRepetitionBase"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una classe base per le ripetizioni in un modello di ricorrenza giornaliera."
type: docs
weight: 65
url: /it/java/com.aspose.tasks/dailyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class DailyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Rappresenta una classe base per le ripetizioni in un modello di ricorrenza giornaliera.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Ottiene un numero di giorni che rappresenta l'intervallo in giorni tra le occorrenze. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Imposta un numero di giorni che rappresenta l'intervallo in giorni tra le occorrenze. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


Ottiene un calcolatore utilizzato per calcolare una ripetizione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


Ottiene un numero di giorni che rappresenta l'intervallo in giorni tra le occorrenze.

**Returns:**
int - un numero di giorni che rappresenta l'intervallo in giorni tra le occorrenze.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


Ottiene un validatore per il modello di ricorrenza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


Imposta un numero di giorni che rappresenta l'intervallo in giorni tra le occorrenze.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un numero di giorni che rappresenta l'intervallo in giorni tra le occorrenze. |

