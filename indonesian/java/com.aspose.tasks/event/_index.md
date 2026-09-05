---
title: "Acara"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Sebuah peristiwa."
type: docs
weight: 374
url: /id/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

Sebuah peristiwa.

`TArgs`: argumen acara.

TArgs :
## Metode

| Metode | Deskripsi |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | Metode ini dipanggil ketika acara dipancarkan. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


Metode ini dipanggil ketika acara dipancarkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pengirim | java.lang.Object | sebuah objek yang memulai peristiwa ini. |
| args | TArgs | argumen khusus. |

