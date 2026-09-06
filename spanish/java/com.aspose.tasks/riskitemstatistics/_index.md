---
title: "RiskItemStatistics"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un elemento que almacena datos estadísticos para la tarea del proyecto analizado."
type: docs
weight: 265
url: /es/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Representa un elemento que almacena datos estadísticos para la tarea del proyecto analizado.
## Métodos

| Método | Descripción |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Obtiene el valor esperado del elemento de riesgo. |
| [getItemType()](#getItemType--) | Obtiene una instancia de la enumeración [RiskItemType](../../com.aspose.tasks/riskitemtype). |
| [getMaximum()](#getMaximum--) | Obtiene el valor máximo que se generó durante la simulación Monte Carlo. |
| [getMinimum()](#getMinimum--) | Obtiene el valor mínimo que se generó durante la simulación Monte Carlo. |
| [getPercentile(int percent)](#getPercentile-int-) | Obtiene un valor por debajo del cual cae un porcentaje especificado de muestras generadas. |
| [getStandardDeviation()](#getStandardDeviation--) | Obtiene la desviación estándar del elemento de riesgo. |
| [toString()](#toString--) | Devuelve una representación corta en cadena de un elemento de riesgo. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Obtiene el valor esperado del elemento de riesgo.

**Returns:**
java.util.Date - el valor esperado del elemento de riesgo.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Obtiene una instancia de la enumeración [RiskItemType](../../com.aspose.tasks/riskitemtype).

**Returns:**
int - una instancia de la enumeración [RiskItemType](../../com.aspose/tasks/riskitemtype).
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Obtiene el valor máximo que se generó durante la simulación Monte Carlo.

**Returns:**
java.util.Date - el valor máximo que se generó durante la simulación Monte Carlo.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Obtiene el valor mínimo que se generó durante la simulación Monte Carlo.

**Returns:**
java.util.Date - el valor mínimo que se generó durante la simulación Monte Carlo.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Obtiene un valor por debajo del cual cae un porcentaje especificado de muestras generadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| porcentaje | int | el porcentaje especificado entre 0 y 100. |

**Returns:**
java.util.Date - un valor por debajo del cual cae un porcentaje especificado de muestras generadas.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Obtiene la desviación estándar del elemento de riesgo.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Devuelve una representación en cadena corta de un elemento de riesgo. Los detalles exactos de la representación no están especificados y pueden cambiar.

**Returns:**
java.lang.String - cadena corta que representa el objeto RiskItem.
