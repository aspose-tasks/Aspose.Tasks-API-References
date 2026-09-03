---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete μέθοδος"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks για C++"
description: "Ενημερώνει όλη τη δουλειά ως ολοκληρωμένη μέσω μιας καθορισμένης ημερομηνίας για ολόκληρο το έργο."
type: docs
weight: 2080
url: /el/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Ενημερώνει όλη τη δουλειά ως ολοκληρωμένη μέσω μιας καθορισμένης ημερομηνίας για ολόκληρο το έργο.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| completeThrough | Η ημερομηνία για την ενημέρωση της εργασίας ως ολοκληρωμένη μέχρι. |
| setZeroOrHundredPercentCompleteOnly | Εάν οριστεί σε true, ενημερώνει μόνο εκείνες τις εργασίες ως 100% ολοκληρωμένες των οποίων η ημερομηνία λήξης είναι πριν από την καθορισμένη ημερομηνία complete-through. Διαφορετικά, υπολογίζει μια τιμή ποσοστού ολοκλήρωσης βάσει της προγραμματισμένης ημερομηνίας έναρξης και των ημερομηνιών complete-through. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Ενημερώνει όλη την εργασία ως ολοκληρωμένη μέχρι μια καθορισμένη ημερομηνία για τη συγκεκριμένη λίστα εργασιών.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| completeThrough | Η ημερομηνία για την ενημέρωση της εργασίας ως ολοκληρωμένη μέχρι. |
| setZeroOrHundredPercentCompleteOnly | Εάν οριστεί σε true, ενημερώνει μόνο εκείνες τις εργασίες ως 100% ολοκληρωμένες των οποίων η ημερομηνία λήξης είναι πριν από την καθορισμένη ημερομηνία complete-through. Διαφορετικά, υπολογίζει μια τιμή ποσοστού ολοκλήρωσης βάσει της προγραμματισμένης ημερομηνίας έναρξης και των ημερομηνιών complete-through. |
| taskCollection | Λίστα< Task > των εργασιών για τις οποίες θα ενημερωθεί η εργασία. |

