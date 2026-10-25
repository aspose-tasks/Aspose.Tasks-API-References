---
title: "Και"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Εφαρμόζει λογικό AND στις καθορισμένες συνθήκες."
type: docs
weight: 10
url: /el/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Εφαρμόζει λογικό AND στις καθορισμένες συνθήκες.

T : Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης And&lt;T&gt;. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [check(T el)](#check-T-) | Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τις συνθήκες. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης And&lt;T&gt;.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | Πρώτη συνθήκη. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | Δεύτερη συνθήκη. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τις συνθήκες.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Το αντικείμενο προς έλεγχο. |

**Returns:**
boolean - True εάν το αντικείμενο ικανοποιεί τις συνθήκες.
