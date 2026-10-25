---
title: "ICondition"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een voorwaarde voor die kan worden gebruikt door filters of zoekmethoden."
type: docs
weight: 377
url: /nl/java/com.aspose.tasks/icondition/
---
```
public interface ICondition<T>
```

Stelt een voorwaarde voor die kan worden gebruikt door filters of zoekmethoden.

T : Het type object waarop de methode‑interface moet worden toegepast.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [check(T el)](#check-T-) | Retourneert true als het opgegeven object aan de voorwaarden voldoet. |
### check(T el) {#check-T-}
```
public abstract boolean check(T el)
```


Retourneert true als het opgegeven object aan de voorwaarden voldoet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Het object om te controleren. |

**Returns:**
boolean - True als het object aan de voorwaarden voldoet.
