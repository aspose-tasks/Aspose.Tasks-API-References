---
title: "TreeAlgorithmBase"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas dasar untuk implementasi ITreeAlgorithmltTgt"
type: docs
weight: 327
url: /id/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

Kelas dasar untuk implementasi ITreeAlgorithm<T>.

T : Tipe elemen.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Memproses sebuah node pada pohon. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Dipanggil setelah memproses sebuah node pada pohon. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Dipanggil sebelum memproses sebuah node pada pohon. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Memproses sebuah node pada pohon.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Node untuk diproses. |
| tingkat | int | Level node pohon. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public void postAlg(T el, int level)
```


Dipanggil setelah memproses sebuah node pada pohon.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Node untuk diproses. |
| tingkat | int | Level node pohon. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Dipanggil sebelum memproses sebuah node pada pohon.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Node untuk diproses. |
| tingkat | int | Level node pohon. |

