---
title: "TaskUtils"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Βοηθητική κλάση που παρέχει χρήσιμες λειτουργίες με εργασίες."
type: docs
weight: 307
url: /el/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Βοηθητική κλάση που παρέχει χρήσιμες λειτουργίες με εργασίες.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Εφαρμόζει τον καθορισμένο αλγόριθμο σε κάθε εργασία ενός δέντρου. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Δημιουργεί νέο δέντρο εργασιών που ικανοποιούν την προϋπόθεση. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Βρίσκει μια εργασία που ικανοποιεί την προϋπόθεση σε ένα δέντρο εργασιών. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Υπολογίζει αναδρομικά τον αριθμό των παιδικών εργασιών μιας εργασίας σε όλα τα επίπεδα. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Εφαρμόζει τον καθορισμένο αλγόριθμο σε κάθε εργασία ενός δέντρου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Ρίζα του δέντρου |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Εφαρμοσμένος αλγόριθμος. |
| επίπεδο | int | Επίπεδο της ρίζας της εργασίας. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Δημιουργεί νέο δέντρο εργασιών που ικανοποιούν την προϋπόθεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Ρίζα του δέντρου. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Εφαρμοσμένη προϋπόθεση. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Βρίσκει μια εργασία που ικανοποιεί την προϋπόθεση σε ένα δέντρο εργασιών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Ρίζα του δέντρου. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Εφαρμοσμένη προϋπόθεση. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Υπολογίζει αναδρομικά τον αριθμό των παιδικών εργασιών μιας εργασίας σε όλα τα επίπεδα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Η εργασία της οποίας υπολογίζονται τα παιδιά. |

**Returns:**
int - Ο αριθμός των παιδιών.
