---
title: "No"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Aplica NOT lógico a la condición especificada."
type: docs
weight: 162
url: /es/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Aplica NOT lógico a la condición especificada.

T : El tipo de objeto al que aplicar la interfaz del método.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Inicializa una nueva instancia de la clase Not&lt;T&gt;. |
## Métodos

| Método | Descripción |
| --- | --- |
| [check(T el)](#check-T-) | Devuelve true si el objeto especificado satisface la condición. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Inicializa una nueva instancia de la clase Not&lt;T&gt;.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Condición especificada. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Devuelve true si el objeto especificado satisface la condición.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | El objeto a comprobar. |

**Returns:**
boolean - True si el objeto satisface la condición.
