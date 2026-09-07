---
title: "ResourceLeveler.ClearLeveling"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceLeveler. Καθαρίζει οποιαδήποτε καθυστέρηση εξισορρόπησης που είχε προστεθεί προηγουμένως στο έργο κατά τη διάρκεια της εξισορρόπησης πόρων."
type: docs
weight: 10
url: /el/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Καθαρίζει οποιαδήποτε καθυστέρηση ισοστάθμισης που είχε προστεθεί προηγουμένως στο έργο κατά τη διάρκεια της ισοστάθμισης πόρων.

```csharp
public static void ClearLeveling(Project project)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | Project | Έργο για εκκαθάριση εξισορρόπησης. |

## Παραδείγματα

Δείχνει πώς να ισοσταθμίσετε όλους τους πόρους του έργου χρησιμοποιώντας τις προεπιλεγμένες επιλογές.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### Δείτε επίσης

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Καθαρίζει οποιαδήποτε καθυστέρηση ισοστάθμισης που είχε προστεθεί προηγουμένως στις καθορισμένες εργασίες κατά τη διάρκεια της ισοστάθμισης πόρων.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| εργασίες | IEnumerable`1 | Η συλλογή που περιέχει τις εργασίες για τις οποίες πρέπει να καθαριστεί η καθυστέρηση εξισορρόπησης. |

### Δείτε επίσης

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


