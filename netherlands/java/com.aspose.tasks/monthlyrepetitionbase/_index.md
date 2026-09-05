---
title: "MonthlyRepetitionBase"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een basispatroon voor de maandelijkse dagpositie voor."
type: docs
weight: 159
url: /nl/java/com.aspose.tasks/monthlyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class MonthlyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Stelt een basispatroon voor de maandelijkse dagpositie voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Haalt een aantal maanden op dat het interval in maanden tussen gebeurtenissen vertegenwoordigt. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Stelt een aantal maanden in dat het interval in maanden tussen gebeurtenissen vertegenwoordigt. |
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


Haalt een aantal maanden op dat het interval in maanden tussen gebeurtenissen vertegenwoordigt.

**Returns:**
int - een aantal maanden dat het interval in maanden tussen gebeurtenissen vertegenwoordigt.
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


Stelt een aantal maanden in dat het interval in maanden tussen gebeurtenissen vertegenwoordigt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een aantal maanden dat het interval in maanden tussen gebeurtenissen vertegenwoordigt. |

