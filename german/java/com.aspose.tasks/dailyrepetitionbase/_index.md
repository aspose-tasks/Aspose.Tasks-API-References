---
title: "DailyRepetitionBase"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Basisklasse für Wiederholungen im täglichen Wiederholungsmuster dar."
type: docs
weight: 65
url: /de/java/com.aspose.tasks/dailyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class DailyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Stellt eine Basisklasse für Wiederholungen im täglichen Wiederholungsmuster dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Gibt eine Anzahl von Tagen zurück, die das Intervall in Tagen zwischen den Vorkommen darstellt. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Legt eine Anzahl von Tagen fest, die das Intervall in Tagen zwischen den Vorkommen darstellt. |
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


Gibt eine Anzahl von Tagen zurück, die das Intervall in Tagen zwischen den Vorkommen darstellt.

**Returns:**
int - eine Anzahl von Tagen, die das Intervall in Tagen zwischen den Vorkommen darstellt.
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


Legt eine Anzahl von Tagen fest, die das Intervall in Tagen zwischen den Vorkommen darstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Tagen, die das Intervall in Tagen zwischen den Vorkommen darstellt. |

