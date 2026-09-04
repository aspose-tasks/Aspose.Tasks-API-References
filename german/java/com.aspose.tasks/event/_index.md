---
title: "Ereignis"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ein Ereignis."
type: docs
weight: 374
url: /de/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

Ein Ereignis.

`TArgs`: Ereignisargumente.

TArgs :
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Diese Methode wird aufgerufen, wenn das Ereignis ausgelöst wird. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Diese Methode wird aufgerufen, wenn das Ereignis ausgelöst wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | java.lang.Object | ein Objekt, das dieses Ereignis auslöst. |
| args | TArgs | benutzerdefinierte Argumente. |

