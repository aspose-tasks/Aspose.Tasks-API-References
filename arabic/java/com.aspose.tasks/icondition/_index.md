---
title: "ICondition"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل شرطًا يمكن استخدامه بواسطة الفلاتر أو طرق البحث."
type: docs
weight: 377
url: /ar/java/com.aspose.tasks/icondition/
---
```
public interface ICondition<T>
```

يمثل شرطًا يمكن استخدامه بواسطة الفلاتر أو طرق البحث.

T : نوع الكائن الذي سيتم تطبيق واجهة الطريقة عليه.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [check(T el)](#check-T-) | يرجع true إذا كان الكائن المحدد يحقق الشروط. |
### check(T el) {#check-T-}
```
public abstract boolean check(T el)
```


يرجع true إذا كان الكائن المحدد يحقق الشروط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| el | T | الكائن المراد فحصه. |

**Returns:**
boolean - True إذا كان الكائن يحقق الشروط.
