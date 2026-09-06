---
title: "Y"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Aplica AND lógico a las condiciones especificadas."
type: docs
weight: 10
url: /es/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Aplica AND lógico a las condiciones especificadas.

T : El tipo de objeto al que aplicar la interfaz del método.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | Inicializa una nueva instancia de la clase And&lt;T&gt;. |
## Métodos

| Método | Descripción |
| --- | --- |
| [check(T el)](#check-T-) | Devuelve verdadero si el objeto especificado cumple las condiciones. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


Inicializa una nueva instancia de la clase And&lt;T&gt;.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | Primera condición. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | Segunda condición. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Devuelve verdadero si el objeto especificado cumple las condiciones.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | El objeto a comprobar. |

**Returns:**
boolean - Verdadero si el objeto cumple las condiciones.
