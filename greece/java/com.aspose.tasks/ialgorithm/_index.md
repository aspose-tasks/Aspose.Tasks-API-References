---
title: "IAlgorithm"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει έναν αλγόριθμο που μπορεί να εφαρμοστεί σε μια λίστα αντικειμένων T."
type: docs
weight: 375
url: /el/java/com.aspose.tasks/ialgorithm/
---
```
public interface IAlgorithm<T>
```

Αναπαριστά έναν αλγόριθμο που μπορεί να εφαρμοστεί σε μια λίστα αντικειμένων `T`.

T : Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [alg(T el, int index)](#alg-T-int-) | Επεξεργάζεται ένα αντικείμενο στη λίστα. |
| [postAlg(T el, int index)](#postAlg-T-int-) | Καλείται μετά την επεξεργασία ενός αντικειμένου. |
| [preAlg(T el, int index)](#preAlg-T-int-) | Καλείται πριν την επεξεργασία ενός αντικειμένου. |
### alg(T el, int index) {#alg-T-int-}
```
public abstract void alg(T el, int index)
```


Επεξεργάζεται ένα αντικείμενο στη λίστα. Καλείται μετά το [preAlg(T, int)](../../com.aspose.tasks/ialgorithm\#preAlg-T--int-);

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Επεξεργασμένο αντικείμενο. |
| index | int | Δείκτης του αντικειμένου. |

### postAlg(T el, int index) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int index)
```


Καλείται μετά την επεξεργασία ενός αντικειμένου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Επεξεργασμένο αντικείμενο. |
| index | int | Δείκτης του αντικειμένου. |

### preAlg(T el, int index) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int index)
```


Καλείται πριν την επεξεργασία ενός αντικειμένου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Επεξεργασμένο αντικείμενο. |
| index | int | Δείκτης του αντικειμένου. |

