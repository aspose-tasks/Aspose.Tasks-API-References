---
title: "ResourceLeveler.LevelResources"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceLeveler. Εξισορροπεί τις εργασίες για τους καθορισμένους πόρους χρησιμοποιώντας τις καθορισμένες επιλογές εξισορρόπησης."
type: docs
weight: 30
url: /el/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Ισοσταθμίζει εργασίες για τους καθορισμένους πόρους χρησιμοποιώντας τις καθορισμένες επιλογές ισοστάθμισης.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | Project | Έργο για εφαρμογή εξισορρόπησης πόρων. |
| επιλογές | LevelingOptions | Επιλογές που καθορίζουν πώς να εξισορροπηθούν οι πόροι. |

### Τιμή Επιστροφής

Αντικείμενο που περιέχει τα αποτελέσματα της εξισορρόπησης πόρων.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | αν η παράμετρος options είναι null. |

## Παραδείγματα

Δείχνει πώς να εξισορροπεί συγκεκριμένο πόρο, να προσαρμόζει τις επιλογές εξισορρόπησης και να εξετάζει τα μηνύματα του αλγορίθμου εξισορρόπησης.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### Δείτε επίσης

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


