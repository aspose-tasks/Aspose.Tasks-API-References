---
title: "Project.DisplayOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει μια παρουσία της κλάσης ProjectDisplayOptions"
type: docs
weight: 380
url: /el/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

Λαμβάνει μια παρουσία της κλάσης [`ProjectDisplayOptions`](../../projectdisplayoptions/).

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## Παραδείγματα

Δείχνει πώς να ρυθμίσετε τις επιλογές εμφάνισης του project.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζονται προειδοποιήσεις όταν το Project εντοπίζει πιθανή σύγκρουση χρονοπρογραμματισμού με μια χειροκίνητα προγραμματισμένη εργασία.
// Αυτή η επιλογή είναι διαθέσιμη για την έκδοση Project 2010 και μεταγενέστερες.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### Δείτε επίσης

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


