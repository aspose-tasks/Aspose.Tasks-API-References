---
title: "AndAllCondition"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Past logische EN toe op alle voorwaarden."
type: docs
weight: 11
url: /nl/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Past logische AND toe op alle voorwaarden. Bijvoorbeeld: cond1 AND cond2 AND cond3...

T : Het type object waarop de methode‑interface moet worden toegepast.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Initialiseert een nieuw exemplaar van de AndAllCondition&lt;T&gt; klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [check(T el)](#check-T-) | Retourneert true als het opgegeven object aan de voorwaarden voldoet. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Initialiseert een nieuw exemplaar van de AndAllCondition&lt;T&gt; klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| voorwaarden | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | De lijst met voorwaarden. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Retourneert true als het opgegeven object aan de voorwaarden voldoet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Het object om te controleren. |

**Returns:**
boolean - True als het object aan de voorwaarden voldoet.
