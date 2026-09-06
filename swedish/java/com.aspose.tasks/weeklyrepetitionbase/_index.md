---
title: "WeeklyRepetitionBase"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en basklass för upprepningar i ett veckovis återkomstande mönster."
type: docs
weight: 358
url: /sv/java/com.aspose.tasks/weeklyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class WeeklyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Representerar en basklass för upprepningar i ett veckovis återkomstande mönster.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Hämtar ett antal veckor som representerar intervallet i veckor mellan förekomster. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Ställer in ett antal veckor som representerar intervallet i veckor mellan förekomster. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


Hämtar en kalkylator som används för att beräkna en repetition.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


Hämtar ett antal veckor som representerar intervallet i veckor mellan förekomster.

**Returns:**
int - ett antal veckor som representerar intervallet i veckor mellan förekomster.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


Hämtar en validator för återkomstmönster.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


Ställer in ett antal veckor som representerar intervallet i veckor mellan förekomster.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett antal veckor som representerar intervallet i veckor mellan förekomster. |

