---
title: "Och"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillämpar logisk OCH på de angivna villkoren."
type: docs
weight: 10
url: /sv/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Tillämpar logisk OCH på de angivna villkoren.

T : Typen av objekt som metodgränssnittet ska tillämpas på.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | Initierar en ny instans av klassen And&lt;T&gt;. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [check(T el)](#check-T-) | Returnerar true om det angivna objektet uppfyller villkoren. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


Initierar en ny instans av klassen And&lt;T&gt;.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | Första villkoret. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | Andra villkoret. |

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
