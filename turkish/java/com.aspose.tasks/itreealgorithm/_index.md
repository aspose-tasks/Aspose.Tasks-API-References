---
title: "ITreeAlgorithm"
second_title: "Aspose.Tasks for Java API Referansı"
description: "T nesnelerinin bir ağacına uygulanabilen bir algoritmayı temsil eder."
type: docs
weight: 384
url: /tr/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

`T` nesneler ağacına uygulanabilen bir algoritmayı temsil eder.

T : Uygulama yöntemi arayüzünün uygulanacağı nesnenin türü.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Bir ağacın düğümünü işler. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Bir ağacın düğümünün işlenmesinden sonra çağrılır. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Bir ağacın düğümünün işlenmesinden önce çağrılır. |
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
public abstract void postAlg(T el, int level)
```


Bir ağacın düğümünün işlenmesinden sonra çağrılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | İşlenecek düğüm. |
| seviye | int | Ağaç düğüm seviyesi. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Bir ağacın düğümünün işlenmesinden önce çağrılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | İşlenecek düğüm. |
| seviye | int | Ağaç düğüm seviyesi. |

