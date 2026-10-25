---
title: "TreeAlgorithmBase"
second_title: "Aspose.Tasks for Java API Referansı"
description: "ITreeAlgorithmltTgt uygulamaları için bir temel sınıf"
type: docs
weight: 327
url: /tr/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

ITreeAlgorithm&lt;T&gt; uygulamaları için temel sınıf.

T : Elemanların tipi.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Bir ağacın düğümünü işler. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Bir ağacın düğümünün işlenmesinden sonra çağrılır. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Bir ağacın düğümünün işlenmesinden önce çağrılır. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Bir ağacın düğümünü işler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | İşlenecek düğüm. |
| seviye | int | Ağaç düğüm seviyesi. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public void postAlg(T el, int level)
```


Bir ağacın düğümünün işlenmesinden sonra çağrılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | İşlenecek düğüm. |
| seviye | int | Ağaç düğüm seviyesi. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Bir ağacın düğümünün işlenmesinden önce çağrılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | İşlenecek düğüm. |
| seviye | int | Ağaç düğüm seviyesi. |

