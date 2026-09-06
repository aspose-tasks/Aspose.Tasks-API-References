---
title: "AndAllCondition"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Tüm koşullara mantıksal VE uygular."
type: docs
weight: 11
url: /tr/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Tüm koşullara mantıksal AND uygular. Örneğin: cond1 AND cond2 AND cond3...

T : Uygulama yöntemi arayüzünün uygulanacağı nesnenin türü.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Yeni bir AndAllCondition&lt;T&gt; sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [check(T el)](#check-T-) | Belirtilen nesne koşulları karşılıyorsa true döndürür. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Yeni bir AndAllCondition&lt;T&gt; sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| koşullar | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | Koşulların listesi. |

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
