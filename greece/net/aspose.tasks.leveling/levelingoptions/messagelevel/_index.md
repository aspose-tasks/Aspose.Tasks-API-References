---
title: "LevelingOptions.MessageLevel"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα LevelingOptions. Λαμβάνει ή ορίζει το επίπεδο των μηνυμάτων καταγραφής που εκδίδονται από το Aspose.Tasks κατά την εξισορρόπηση πόρων"
type: docs
weight: 60
url: /el/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Λαμβάνει ή ορίζει το επίπεδο των μηνυμάτων καταγραφής που εκδίδονται από το Aspose.Tasks κατά τη διάρκεια της ισοστάθμισης πόρων.

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


