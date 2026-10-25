---
title: "ITreeAlgorithm"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά έναν αλγόριθμο που μπορεί να εφαρμοστεί σε ένα δέντρο αντικειμένων T."
type: docs
weight: 384
url: /el/java/com.aspose.tasks/itreealgorithm/
---
```
public interface ITreeAlgorithm<T>
```

Αντιπροσωπεύει έναν αλγόριθμο που μπορεί να εφαρμοστεί σε ένα δέντρο αντικειμένων `T`.

T : Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Επεξεργάζεται έναν κόμβο ενός δέντρου. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Καλείται μετά την επεξεργασία ενός κόμβου ενός δέντρου. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Καλείται πριν από την επεξεργασία ενός κόμβου ενός δέντρου. |
### alg(T el, int level) {#alg-T-int-}
```
public abstract void alg(T el, int level)
```


Επεξεργάζεται έναν κόμβο ενός δέντρου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Κόμβος προς επεξεργασία. |
| επίπεδο | int | Επίπεδο κόμβου δέντρου. |

### postAlg(T el, int level) {#postAlg-T-int-}
```
public abstract void postAlg(T el, int level)
```


Καλείται μετά την επεξεργασία ενός κόμβου ενός δέντρου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Κόμβος προς επεξεργασία. |
| επίπεδο | int | Επίπεδο κόμβου δέντρου. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public abstract void preAlg(T el, int level)
```


Καλείται πριν από την επεξεργασία ενός κόμβου ενός δέντρου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Κόμβος προς επεξεργασία. |
| επίπεδο | int | Επίπεδο κόμβου δέντρου. |

