---
title: "LevelingOptions.MessageHandler"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα LevelingOptions. Λαμβάνει ή ορίζει την κλήση επανάκλησης διαχειριστή μηνυμάτων που μπορεί να χρησιμοποιηθεί για την παρέμβαση στα μηνύματα καταγραφής που παράγονται από το Aspose.Tasks κατά την εξισορρόπηση πόρων"
type: docs
weight: 50
url: /el/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

Λαμβάνει ή ορίζει την κλήση επανάκλησης του διαχειριστή μηνυμάτων που μπορεί να χρησιμοποιηθεί για την παρέμβαση σε μηνύματα καταγραφής που παράγονται από το Aspose.Tasks κατά τη διάρκεια της ισοστάθμισης πόρων.

```csharp
public IMessageHandler MessageHandler { get; set; }
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

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


