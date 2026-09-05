---
title: "ITreeAlgorithm"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili sebuah algoritma yang dapat diterapkan pada pohon objek T."
type: docs
weight: 384
url: /id/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

Mewakili algoritma yang dapat diterapkan pada pohon objek `T`.

T : Tipe objek untuk menerapkan antarmuka metode ke.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Memproses sebuah node pada pohon. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Dipanggil setelah memproses sebuah node pada pohon. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Dipanggil sebelum memproses sebuah node pada pohon. |
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
public abstract void postAlg(T el, int level)
```


Dipanggil setelah memproses sebuah node pada pohon.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Node untuk diproses. |
| tingkat | int | Level node pohon. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Dipanggil sebelum memproses sebuah node pada pohon.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Node untuk diproses. |
| tingkat | int | Level node pohon. |

