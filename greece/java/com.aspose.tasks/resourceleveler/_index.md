---
title: "ResourceLeveler"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Περιέχει μεθόδους εξισορρόπησης πόρων."
type: docs
weight: 253
url: /el/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Περιέχει μεθόδους εξισορρόπησης πόρων.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Καθαρίζει οποιαδήποτε καθυστέρηση εξισορρόπησης που είχε προστεθεί προηγουμένως στο έργο κατά τη διάρκεια της εξισορρόπησης πόρων. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Καθαρίζει οποιαδήποτε καθυστέρηση εξισορρόπησης που είχε προστεθεί προηγουμένως στις καθορισμένες εργασίες κατά τη διάρκεια της εξισορρόπησης πόρων. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Εξισορροπεί τις εργασίες για όλους τους πόρους του έργου χρησιμοποιώντας τις προεπιλεγμένες επιλογές εξισορρόπησης. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Εξισορροπεί τις εργασίες για τους καθορισμένους πόρους χρησιμοποιώντας τις καθορισμένες επιλογές εξισορρόπησης. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Καθαρίζει οποιαδήποτε καθυστέρηση εξισορρόπησης που είχε προστεθεί προηγουμένως στο έργο κατά τη διάρκεια της εξισορρόπησης πόρων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Έργο για την εκκαθάριση της εξισορρόπησης. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Καθαρίζει οποιαδήποτε καθυστέρηση εξισορρόπησης που είχε προστεθεί προηγουμένως στις καθορισμένες εργασίες κατά τη διάρκεια της εξισορρόπησης πόρων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| εργασίες | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | Η συλλογή που περιέχει εργασίες για τις οποίες πρέπει να καθαριστεί η καθυστέρηση εξισορρόπησης. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Εξισορροπεί τις εργασίες για όλους τους πόρους του έργου χρησιμοποιώντας τις προεπιλεγμένες επιλογές εξισορρόπησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Έργο για την εφαρμογή εξισορρόπησης πόρων. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Εξισορροπεί τις εργασίες για τους καθορισμένους πόρους χρησιμοποιώντας τις καθορισμένες επιλογές εξισορρόπησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Έργο για την εφαρμογή εξισορρόπησης πόρων. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Επιλογές που καθορίζουν πώς να εξισορροπηθούν οι πόροι. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
