---
title: "DailyRepetitionBase"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Vertegenwoordigt een basisklasse voor herhalingen in een dagelijks terugkeerpatroon."
type: docs
weight: 65
url: /nl/java/com.aspose.tasks/dailyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class DailyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Vertegenwoordigt een basisklasse voor herhalingen in een dagelijks terugkeerpatroon.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Haalt een aantal dagen op dat de interval in dagen tussen gebeurtenissen vertegenwoordigt. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Stelt een aantal dagen in dat de interval in dagen tussen gebeurtenissen vertegenwoordigt. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


Haalt een rekenmachine op die wordt gebruikt om een herhaling te berekenen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


Haalt een aantal dagen op dat de interval in dagen tussen gebeurtenissen vertegenwoordigt.

**Returns:**
int - een aantal dagen dat de interval in dagen tussen gebeurtenissen vertegenwoordigt.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


Haalt een validator op voor het herhalingspatroon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


Stelt een aantal dagen in dat de interval in dagen tussen gebeurtenissen vertegenwoordigt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal dagen dat de interval in dagen tussen gebeurtenissen vertegenwoordigt. |

