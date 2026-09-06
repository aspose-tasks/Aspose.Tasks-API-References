---
title: "AndAllCondition"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Aplica AND lógico a todas las condiciones."
type: docs
weight: 11
url: /es/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Aplica AND lógico a todas las condiciones. Por ejemplo: cond1 AND cond2 AND cond3...

T : El tipo de objeto al que aplicar la interfaz del método.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Inicializa una nueva instancia de la clase AndAllCondition&lt;T&gt;. |
## Métodos

| Método | Descripción |
| --- | --- |
| [check(T el)](#check-T-) | Devuelve verdadero si el objeto especificado cumple las condiciones. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Inicializa una nueva instancia de la clase AndAllCondition&lt;T&gt;.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| condiciones | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | La lista de condiciones. |

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
