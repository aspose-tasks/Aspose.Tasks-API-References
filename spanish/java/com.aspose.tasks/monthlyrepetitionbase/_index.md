---
title: "MonthlyRepetitionBase"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un patrón base para la posición del día mensual."
type: docs
weight: 159
url: /es/java/com.aspose.tasks/monthlyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class MonthlyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Representa un patrón base para la posición del día mensual.
## Métodos

| Método | Descripción |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Obtiene un número de mes que representa el intervalo en meses entre ocurrencias. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Establece un número de mes que representa el intervalo en meses entre ocurrencias. |
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


Obtiene un número de mes que representa el intervalo en meses entre ocurrencias.

**Returns:**
int - un número de mes que representa el intervalo en meses entre ocurrencias.
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


Establece un número de mes que representa el intervalo en meses entre ocurrencias.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un número de mes que representa el intervalo en meses entre ocurrencias. |

