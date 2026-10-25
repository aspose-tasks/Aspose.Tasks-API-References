---
title: "Evento"
second_title: "Aspose.Tasks for Java API Reference"
description: "Un evento."
type: docs
weight: 374
url: /it/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

Un evento.

`TArgs`: argomenti dell'evento.

TArgs :
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Questo metodo viene invocato quando l'evento viene emesso. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Questo metodo viene invocato quando l'evento viene emesso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mittente | java.lang.Object | un oggetto che avvia questo evento. |
| args | TArgs | argomenti personalizzati. |

