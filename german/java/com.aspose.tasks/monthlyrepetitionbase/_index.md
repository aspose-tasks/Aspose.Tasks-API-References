---
title: "MonthlyRepetitionBase"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt ein Basismuster für die Position des Tages im Monat dar."
type: docs
weight: 159
url: /de/java/com.aspose.tasks/monthlyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class MonthlyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Stellt ein Basismuster für die Position des Tages im Monat dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Ruft eine Monatszahl ab, die das Intervall in Monaten zwischen den Vorkommnissen darstellt. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Legt eine Anzahl von Monaten fest, die das Intervall in Monaten zwischen den Vorkommnissen darstellt. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


Gibt einen Rechner zurück, der zur Berechnung einer Wiederholung verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


Ruft eine Monatszahl ab, die das Intervall in Monaten zwischen den Vorkommnissen darstellt.

**Returns:**
int - eine Anzahl von Monaten, die das Intervall in Monaten zwischen den Vorkommnissen darstellt.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


Gibt einen Validator für das Wiederholungsmuster zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


Legt eine Anzahl von Monaten fest, die das Intervall in Monaten zwischen den Vorkommnissen darstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Monaten, die das Intervall in Monaten zwischen den Vorkommnissen darstellt. |

