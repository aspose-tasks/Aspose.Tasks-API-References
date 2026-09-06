---
title: "Değil"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Belirtilen koşula mantıksal NOT uygular."
type: docs
weight: 162
url: /tr/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Belirtilen koşula mantıksal NOT uygular.

T : Uygulama yöntemi arayüzünün uygulanacağı nesnenin türü.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Not&lt;T&gt; sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [check(T el)](#check-T-) | Belirtilen nesne koşulu sağlarsa true döndürür. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Not&lt;T&gt; sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Belirtilen koşul. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Belirtilen nesne koşulu sağlarsa true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | Kontrol edilecek nesne. |

**Returns:**
boolean - Nesne koşulu sağlarsa True.
