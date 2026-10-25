---
title: "ArrayUtils"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Κλάση βοηθητική για επεξεργασία ArrayList."
type: docs
weight: 14
url: /el/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

Κλάση βοηθητική για επεξεργασία ArrayList.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Εφαρμόστε αλγόριθμο για κάθε στοιχείο λίστας ξεκινώντας από τη συγκεκριμένη θέση. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | Φιλτράρετε τα στοιχεία του ArrayList με βάση την καθορισμένη συνθήκη. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Βρείτε την πρώτη εμφάνιση ενός στοιχείου ArrayList που ικανοποιεί την καθορισμένη συνθήκη. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| πίνακες | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Εφαρμόστε αλγόριθμο για κάθε στοιχείο λίστας ξεκινώντας από τη συγκεκριμένη θέση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πίνακας | java.util.List | ArrayList προς επεξεργασία. |
| αλγόριθμος | com.aspose.tasks.IAlgorithm | Εφαρμοσμένος αλγόριθμος. |
| startIndex | int | Θέση αρχικού στοιχείου. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


Φιλτράρετε τα στοιχεία του ArrayList με βάση την καθορισμένη συνθήκη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πίνακας | java.util.List | Λίστα προς επεξεργασία. |
| cond | com.aspose.tasks.ICondition | Συνθήκη που χρησιμοποιείται για το φιλτράρισμα της λίστας. |

**Returns:**
java.util.List - Φιλτραρισμένη λίστα.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Βρείτε την πρώτη εμφάνιση ενός στοιχείου ArrayList που ικανοποιεί την καθορισμένη συνθήκη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πίνακας | java.util.List | ArrayList προς επεξεργασία. |
| cond | com.aspose.tasks.ICondition | Συνθήκη που χρησιμοποιείται για την εύρεση στοιχείου ArrayList. |

**Returns:**
java.lang.Object - Στοιχείο λίστας ή null.
