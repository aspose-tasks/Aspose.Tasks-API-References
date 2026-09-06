---
title: "Olay"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir olay."
type: docs
weight: 374
url: /tr/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

Bir olay.

`TArgs`: olay argümanları.

TArgs :
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Bu yöntem, olay yayılınca çağrılır. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Bu yöntem, olay yayılınca çağrılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sender | java.lang.Object | bu olayı başlatan bir nesne. |
| args | TArgs | custom arguments. |

