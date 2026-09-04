---
title: "Όχι"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Εφαρμόζει λογικό NOT στην καθορισμένη συνθήκη."
type: docs
weight: 162
url: /el/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Εφαρμόζει λογικό NOT στην καθορισμένη συνθήκη.

T : Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Αρχικοποιεί μια νέα παρουσία της κλάσης Not&lt;T&gt;. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [check(T el)](#check-T-) | Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τη συνθήκη. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης Not&lt;T&gt;.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Καθορισμένη συνθήκη. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τη συνθήκη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Το αντικείμενο προς έλεγχο. |

**Returns:**
boolean - True εάν το αντικείμενο ικανοποιεί τη συνθήκη.
