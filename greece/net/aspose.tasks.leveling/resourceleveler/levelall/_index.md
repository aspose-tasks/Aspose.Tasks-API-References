---
title: "ResourceLeveler.LevelAll"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceLeveler. Εξισορροπεί τις εργασίες για όλους τους πόρους των έργων χρησιμοποιώντας τις προεπιλεγμένες επιλογές εξισορρόπησης."
type: docs
weight: 20
url: /el/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Ισοσταθμίζει εργασίες για όλους τους πόρους του έργου χρησιμοποιώντας τις προεπιλεγμένες επιλογές ισοστάθμισης.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | Project | Έργο για εφαρμογή εξισορρόπησης πόρων. |

### Τιμή Επιστροφής

Αντικείμενο που περιέχει τα αποτελέσματα της εξισορρόπησης πόρων.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


