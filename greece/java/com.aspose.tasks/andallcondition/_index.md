---
title: "AndAllCondition"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Εφαρμόζει λογικό AND σε όλες τις συνθήκες."
type: docs
weight: 11
url: /el/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Εφαρμόζει λογικό AND σε όλες τις συνθήκες. Για παράδειγμα: cond1 AND cond2 AND cond3...

T : Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Δημιουργεί ένα νέο στιγμιότυπο της κλάσης AndAllCondition&lt;T&gt;. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [check(T el)](#check-T-) | Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τις συνθήκες. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Δημιουργεί ένα νέο στιγμιότυπο της κλάσης AndAllCondition&lt;T&gt;.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| συνθήκες | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | Η λίστα των συνθηκών. |

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
