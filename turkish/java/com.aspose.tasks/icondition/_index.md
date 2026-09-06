---
title: "ICondition"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Filtreler veya arama yöntemleri tarafından kullanılabilecek bir koşulu temsil eder."
type: docs
weight: 377
url: /tr/java/com.aspose.tasks/icondition/
---
```
public interface ICondition<T>
```

Filtreler veya arama yöntemleri tarafından kullanılabilecek bir koşulu temsil eder.

T : Uygulama yöntemi arayüzünün uygulanacağı nesnenin türü.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [check(T el)](#check-T-) | Belirtilen nesne koşulları karşılıyorsa true döndürür. |
### check(T el) {#check-T-}
```
public abstract boolean check(T el)
```


Belirtilen nesne koşulları karşılıyorsa true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | Kontrol edilecek nesne. |

**Returns:**
boolean - Nesne koşulları karşılıyorsa True.
