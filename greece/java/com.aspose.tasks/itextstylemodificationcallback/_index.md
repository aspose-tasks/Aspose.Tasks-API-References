---
title: "ITextStyleModificationCallback"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια κλήση επιστροφής που καλείται πριν εφαρμοστεί το TextStyle σε ένα κελί πίνακα."
type: docs
weight: 383
url: /el/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

Αντιπροσωπεύει μια κλήση επιστροφής που καλείται πριν εφαρμοστεί το TextStyle σε ένα κελί πίνακα.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | Η μέθοδος που θα κληθεί πριν από την απόδοση ενός κελιού πίνακα για μια γραμμή εργασίας στις ακόλουθες προβολές: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


Η μέθοδος που θα κληθεί πριν από την απόδοση ενός κελιού πίνακα για μια γραμμή εργασίας στις ακόλουθες προβολές: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | Το αντικείμενο [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs). |

