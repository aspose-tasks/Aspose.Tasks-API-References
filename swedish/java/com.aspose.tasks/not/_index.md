---
title: "Inte"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillämpar logisk NOT på det angivna villkoret."
type: docs
weight: 162
url: /sv/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Tillämpar logisk NOT på det angivna villkoret.

T : Typen av objekt som metodgränssnittet ska tillämpas på.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Initierar en ny instans av Not&lt;T&gt;-klassen. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [check(T el)](#check-T-) | Returnerar true om det angivna objektet uppfyller villkoret. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Initierar en ny instans av Not&lt;T&gt;-klassen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Angivet villkor. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Returnerar true om det angivna objektet uppfyller villkoret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Objektet som ska kontrolleras. |

**Returns:**
boolean - True om objektet uppfyller villkoret.
