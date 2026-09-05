---
title: "WeeklyRepetitionBase"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een basisklasse voor voor herhalingen in een wekelijks recursiepatroon."
type: docs
weight: 358
url: /nl/java/com.aspose.tasks/weeklyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class WeeklyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Stelt een basisklasse voor voor herhalingen in een wekelijks recursiepatroon.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Haalt een aantal weken op dat het interval in weken tussen gebeurtenissen weergeeft. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Stelt een aantal weken in dat het interval in weken tussen gebeurtenissen weergeeft. |
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


Haalt een aantal weken op dat het interval in weken tussen gebeurtenissen weergeeft.

**Returns:**
int - een aantal weken dat het interval in weken tussen gebeurtenissen weergeeft.
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


Stelt een aantal weken in dat het interval in weken tussen gebeurtenissen weergeeft.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal weken dat het interval in weken tussen gebeurtenissen weergeeft. |

