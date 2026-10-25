---
title: "Κλάση LevelingOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Leveling.LevelingOptions. Επιτρέπει τον καθορισμό παραμέτρων της ισοστάθμισης πόρων"
type: docs
weight: 940
url: /el/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Επιτρέπει τον καθορισμό παραμέτρων της εξισορρόπησης πόρων.

```csharp
public sealed class LevelingOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `LevelingOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Λαμβάνει ή ορίζει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας ισοστάθμισης έργου. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία λήξης της περιόδου ισοστάθμισης. Η προεπιλεγμένη τιμή είναι η ημερομηνία λήξης του έργου. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Λαμβάνει τη σειρά με την οποία ο αλγόριθμος ισοστάθμισης καθυστερεί τις εργασίες που έχουν υπερκατανομές. Μετά τον προσδιορισμό των εργασιών που προκαλούν την υπερκατανομή και των εργασιών που μπορούν να καθυστερηθούν, χρησιμοποιείται η καθορισμένη σειρά για το ποια εργασία πρέπει να καθυστερήσει πρώτη. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Λαμβάνει ή ορίζει την κλήση επανάκλησης του διαχειριστή μηνυμάτων που μπορεί να χρησιμοποιηθεί για την παρέμβαση σε μηνύματα καταγραφής που παράγονται από το Aspose.Tasks κατά τη διάρκεια της ισοστάθμισης πόρων. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Λαμβάνει ή ορίζει το επίπεδο των μηνυμάτων καταγραφής που εκδίδονται από το Aspose.Tasks κατά τη διάρκεια της ισοστάθμισης πόρων. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Λαμβάνει ή ορίζει τη λίστα των πόρων που θα υποβληθούν σε ισοστάθμιση. Εάν οριστεί null, όλοι οι πόροι του έργου θα υποβληθούν σε ισοστάθμιση. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία έναρξης της περιόδου ισοστάθμισης. Η προεπιλεγμένη τιμή είναι η ημερομηνία έναρξης του έργου. |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


