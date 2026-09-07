---
title: "Κλάση LevelingResult"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Leveling.LevelingResult class. Αντιπροσωπεύει τα αποτελέσματα της εξισορρόπησης πόρων"
type: docs
weight: 960
url: /el/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Αντιπροσωπεύει τα αποτελέσματα της εξισορρόπησης πόρων.

```csharp
public sealed class LevelingResult
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [LevelingResult](levelingresult/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `LevelingResult`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Λαμβάνει ένα σύνολο εργασιών που επηρεάζονται από την εξισορρόπηση πόρων. |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


