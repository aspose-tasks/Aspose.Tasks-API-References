---
title: "Ve"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Belirtilen koşullara mantıksal VE uygular."
type: docs
weight: 10
url: /tr/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Belirtilen koşullara mantıksal VE uygular.

T : Uygulama yöntemi arayüzünün uygulanacağı nesnenin türü.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | And&lt;T&gt; sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [check(T el)](#check-T-) | Belirtilen nesne koşulları karşılıyorsa true döndürür. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


And&lt;T&gt; sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | İlk koşul. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | İkinci koşul. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Belirtilen nesne koşulları karşılıyorsa true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | Kontrol edilecek nesne. |

**Returns:**
boolean - Nesne koşulları karşılıyorsa True.
