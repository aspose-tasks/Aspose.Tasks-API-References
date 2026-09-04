---
title: "TreeAlgorithmBase"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Μια βασική κλάση για υλοποιήσεις του ITreeAlgorithmltTgt"
type: docs
weight: 327
url: /el/java/com.aspose.tasks/treealgorithmbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public abstract class TreeAlgorithmBase<T> implements ITreeAlgorithm<T>
```

Μια βασική κλάση για υλοποιήσεις του ITreeAlgorithm<T>

T : Ο τύπος των στοιχείων.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TreeAlgorithmBase()](#TreeAlgorithmBase--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [alg(T el, int level)](#alg-T-int-) | Επεξεργάζεται έναν κόμβο ενός δέντρου. |
| [postAlg(T el, int level)](#postAlg-T-int-) | Καλείται μετά την επεξεργασία ενός κόμβου ενός δέντρου. |
| [preAlg(T el, int level)](#preAlg-T-int-) | Καλείται πριν από την επεξεργασία ενός κόμβου ενός δέντρου. |
### TreeAlgorithmBase() {#TreeAlgorithmBase--}
```
public TreeAlgorithmBase()
```


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
public void postAlg(T el, int level)
```


Καλείται μετά την επεξεργασία ενός κόμβου ενός δέντρου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Κόμβος προς επεξεργασία. |
| επίπεδο | int | Επίπεδο κόμβου δέντρου. |

### preAlg(T el, int level) {#preAlg-T-int-}
```
public void preAlg(T el, int level)
```


Καλείται πριν από την επεξεργασία ενός κόμβου ενός δέντρου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Κόμβος προς επεξεργασία. |
| επίπεδο | int | Επίπεδο κόμβου δέντρου. |

