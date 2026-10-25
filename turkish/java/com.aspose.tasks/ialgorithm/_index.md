---
title: "IAlgorithm"
second_title: "Aspose.Tasks for Java API Referansı"
description: "T nesnelerinin bir listesine uygulanabilen bir algoritmayı temsil eder."
type: docs
weight: 375
url: /tr/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

`T` nesnelerinin listesine uygulanabilen bir algoritmayı temsil eder.

T : Uygulama yöntemi arayüzünün uygulanacağı nesnenin türü.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Listedeki bir nesneyi işler. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Bir nesnenin işlenmesinden sonra çağrılır. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Bir nesnenin işlenmesinden önce çağrılır. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Listedeki bir nesneyi işler. [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-) çağrıldıktan sonra;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | İşlenen nesne. |
| index | int | Nesnenin indeksi. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Bir nesnenin işlenmesinden sonra çağrılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | İşlenen nesne. |
| index | int | Nesnenin indeksi. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Bir nesnenin işlenmesinden önce çağrılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | İşlenen nesne. |
| index | int | Nesnenin indeksi. |

