---
title: "حدث"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "حدث."
type: docs
weight: 374
url: /ar/java/com.aspose.tasks/event/
---
```
public interface Event<TArgs>
```

حدث.

`TArgs`: وسائط الحدث.

TArgs :
## الطرق

| طريقة | الوصف |
| --- | --- |
| [invoke(Object sender, TArgs args)](#invoke-java.lang.Object-TArgs-) | يتم استدعاء هذه الطريقة عندما يتم إصدار الحدث. |
### invoke(Object sender, TArgs args) {#invoke-java.lang.Object-TArgs-}
```
public abstract void invoke(Object sender, TArgs args)
```


يتم استدعاء هذه الطريقة عندما يتم إصدار الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المرسل | java.lang.Object | كائن يطلق هذا الحدث. |
| args | TArgs | معلمات مخصصة. |

