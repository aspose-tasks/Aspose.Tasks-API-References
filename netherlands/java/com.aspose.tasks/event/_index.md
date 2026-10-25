---
title: "Evenement"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Een gebeurtenis."
type: docs
weight: 374
url: /nl/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

Een gebeurtenis.

`TArgs`: gebeurtenisargumenten.

TArgs :
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Deze methode wordt aangeroepen wanneer het evenement wordt uitgezonden. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Deze methode wordt aangeroepen wanneer het evenement wordt uitgezonden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| zender | java.lang.Object | een object dat dit evenement initieert. |
| args | TArgs | aangepaste argumenten. |

