---
title: "Διεπαφή IMessageHandler"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.IMessageHandler interface. Αναπαριστά μια κλήση επιστροφής των αποτελεσμάτων της εξισορρόπησης πόρων"
type: docs
weight: 880
url: /el/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Αναπαριστά μια κλήση επιστροφής για τα αποτελέσματα εξισορρόπησης πόρων.

```csharp
public interface IMessageHandler
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Το Aspose.Tasks καλεί αυτή τη μέθοδο όταν εξάγει ένα μήνυμα. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


