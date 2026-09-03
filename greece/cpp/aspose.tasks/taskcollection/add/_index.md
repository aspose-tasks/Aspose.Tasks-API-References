---
title: "Aspose::Tasks::TaskCollection::Add μέθοδος"
linktitle: "Προσθήκη"
articleTitle: "Προσθήκη"
second_title: "Aspose.Tasks για C++"
description: "Προσθέτει νέα εργασία στη συλλογή εργασιών του έργου στο ίδιο επίπεδο περιγράμματος με την τελευταία εργασία."
type: docs
weight: 10
url: /el/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Προσθέτει νέα εργασία στη συλλογή εργασιών του έργου στο ίδιο επίπεδο περιγράμματος με την τελευταία εργασία.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Εισάγει μια νέα εργασία πριν από μια εργασία με το συγκεκριμένο αναγνωριστικό και στο ίδιο επίπεδο διάρθρωσης.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| παράμετροι | Οι παράμετροι που καθορίζονται για τη δημιουργία επαναλαμβανόμενης εργασίας. |

---

## Add (3 of 5) {#add_3}

Προσθέτει την καθορισμένη εργασία στην παρουσία της κλάσης TaskCollection. Εάν το ParentProject.CalculationMode είναι None, ο χρήστης πρέπει να καλέσει Project.Recalculate() μετά τη χρήση αυτής της μεθόδου (Θα επαναπρογραμματίσει όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργές ημερομηνίες) και θα υπολογίσει τα εξαρτημένα πεδία όπως οι ελεύθεροι χρόνοι, η εργασία και τα πεδία κόστους, τα αναγνωριστικά και τα επίπεδα διάρθρωσης). Εάν το ParentProject.CalculationMode είναι Manual, η μέθοδος θα υπολογίσει μόνο το αναγνωριστικό εργασίας, το επίπεδο διάρθρωσης και τους αριθμούς διάρθρωσης αυτόματα. Εάν το ParentProject.CalculationMode είναι Automatic, η μέθοδος επαναπρογραμματίζει αυτόματα όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργές ημερομηνίες, υπολογίζει ελεύθερους χρόνους, εργασία και πεδία κόστους, επανυπολογίζει τα αναγνωριστικά και τα επίπεδα διάρθρωσης).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| αντικείμενο | η καθορισμένη εργασία που πρέπει να προστεθεί σε αυτή τη συλλογή εργασιών. |

---

## Add (4 of 5) {#add_4}

Προσθέτει μια νέα εργασία στη συλλογή υποεργασιών.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| taskName | το καθορισμένο όνομα εργασίας. |

---

## Add (5 of 5) {#add_5}

Προσθέτει μια νέα επαναλαμβανόμενη εργασία στη συλλογή εργασιών παιδιών.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| taskName | το καθορισμένο όνομα εργασίας. |
| beforeTaskId | Το καθορισμένο αναγνωριστικό μιας εργασίας πριν από την οποία θα εισαχθεί μια νέα εργασία. |

