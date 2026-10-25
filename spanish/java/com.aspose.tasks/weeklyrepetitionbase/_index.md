---
title: "WeeklyRepetitionBase"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una clase base para repeticiones en un patrón de recurrencia semanal."
type: docs
weight: 358
url: /es/java/com.aspose.tasks/weeklyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class WeeklyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Representa una clase base para repeticiones en un patrón de recurrencia semanal.
## Métodos

| Método | Descripción |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Obtiene un número de semanas que representa el intervalo en semanas entre ocurrencias. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Establece un número de semanas que representa el intervalo en semanas entre ocurrencias. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


Obtiene un calculador usado para calcular una repetición.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


Obtiene un número de semanas que representa el intervalo en semanas entre ocurrencias.

**Returns:**
int - un número de semanas que representa el intervalo en semanas entre ocurrencias.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


Obtiene un validador para el patrón de recurrencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


Establece un número de semanas que representa el intervalo en semanas entre ocurrencias.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de semanas que representa el intervalo en semanas entre ocurrencias. |

