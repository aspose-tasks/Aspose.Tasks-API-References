---
title: "ICondition"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett villkor som kan användas av filter eller sökmetoder."
type: docs
weight: 377
url: /sv/java/com.aspose.tasks/icondition/
---
```
public interface ICondition<T>
```

Representerar ett villkor som kan användas av filter eller sökmetoder.

T : Typen av objekt som metodgränssnittet ska tillämpas på.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [check(T el)](#check-T-) | Returnerar true om det angivna objektet uppfyller villkoren. |
### check(T el) {#check-T-}
```
public abstract boolean check(T el)
```


Returnerar true om det angivna objektet uppfyller villkoren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| el | T | Objektet som ska kontrolleras. |

**Returns:**
boolean - True om objektet uppfyller villkoren.
