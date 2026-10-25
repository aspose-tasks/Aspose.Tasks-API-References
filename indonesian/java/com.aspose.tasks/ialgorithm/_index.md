---
title: "IAlgorithm"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili algoritma yang dapat diterapkan pada daftar objek T."
type: docs
weight: 375
url: /id/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

Mewakili algoritma yang dapat diterapkan pada daftar objek `T`.

T : Tipe objek untuk menerapkan antarmuka metode ke.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Memproses sebuah objek dalam daftar. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Dipanggil setelah pemrosesan sebuah objek. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Dipanggil sebelum pemrosesan sebuah objek. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Memproses sebuah objek dalam daftar. Dipanggil setelah [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Objek yang diproses. |
| index | int | Indeks objek. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Dipanggil setelah pemrosesan sebuah objek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Objek yang diproses. |
| index | int | Indeks objek. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Dipanggil sebelum pemrosesan sebuah objek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Objek yang diproses. |
| index | int | Indeks objek. |

