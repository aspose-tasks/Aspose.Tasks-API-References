---
title: "ChildTasksCollector"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Συλλέγει όλες τις υποεργασίες."
type: docs
weight: 49
url: /el/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Συλλέγει όλες τις υποεργασίες.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Επεξεργάζεται το καθορισμένο αντικείμενο. |
| [getTasks()](#getTasks--) | Λαμβάνει μια λίστα με συλλεγμένα αντικείμενα-παιδιά (εργασίες). |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector).

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Επεξεργάζεται το καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Αντικείμενο προς επεξεργασία. |
| επίπεδο | int | Επίπεδο κόμβου δέντρου. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Λαμβάνει μια λίστα με συλλεγμένα αντικείμενα-παιδιά (εργασίες).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - μια λίστα με συλλεγμένα αντικείμενα-παιδιά (εργασίες).
