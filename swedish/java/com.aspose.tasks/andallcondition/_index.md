---
title: "AndAllCondition"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillämpar logisk OCH på alla villkor."
type: docs
weight: 11
url: /sv/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Tillämpar logisk AND på alla villkor. Till exempel: cond1 AND cond2 AND cond3...

T : Typen av objekt som metodgränssnittet ska tillämpas på.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Initierar en ny instans av klassen AndAllCondition&lt;T&gt;. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [check(T el)](#check-T-) | Returnerar true om det angivna objektet uppfyller villkoren. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Initierar en ny instans av klassen AndAllCondition&lt;T&gt;.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| villkor | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | Listan med villkor. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Returnerar true om det angivna objektet uppfyller villkoren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Objektet som ska kontrolleras. |

**Returns:**
boolean - True om objektet uppfyller villkoren.
