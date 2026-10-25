---
title: "ListUtils"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Κλάση βοηθητικού προγράμματος για επεξεργασία λιστών."
type: docs
weight: 147
url: /el/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Κλάση βοηθητικού προγράμματος για επεξεργασία λιστών.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Εφαρμόστε αλγόριθμο για κάθε στοιχείο λίστας ξεκινώντας από τη συγκεκριμένη θέση. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Φιλτράρετε τα στοιχεία της λίστας με βάση την καθορισμένη συνθήκη. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Βρείτε την πρώτη εμφάνιση ενός στοιχείου λίστας που ικανοποιεί την καθορισμένη συνθήκη. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Εφαρμόστε αλγόριθμο για κάθε στοιχείο λίστας ξεκινώντας από τη συγκεκριμένη θέση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| λίστα | java.util.List&lt;T&gt; | Λίστα προς επεξεργασία. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Εφαρμοσμένος αλγόριθμος. |
| startIndex | int | Θέση αρχικού στοιχείου. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Φιλτράρετε τα στοιχεία της λίστας με βάση την καθορισμένη συνθήκη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| λίστα | java.util.List&lt;T&gt; | Μια λίστα προς επεξεργασία. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Συνθήκη που χρησιμοποιείται για το φιλτράρισμα της καθορισμένης λίστας. |

**Returns:**
java.util.List&lt;T&gt; - Φιλτραρισμένη λίστα.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Βρείτε την πρώτη εμφάνιση ενός στοιχείου λίστας που ικανοποιεί την καθορισμένη συνθήκη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| λίστα | java.util.List&lt;T&gt; | Μια λίστα προς επεξεργασία. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Συνθήκη που χρησιμοποιείται για την εύρεση ενός στοιχείου στην καθορισμένη λίστα. |
| clazz | java.lang.Class | Τύπος κλάσης του στοιχείου T. |

**Returns:**
T - Στοιχείο λίστας ή null.
