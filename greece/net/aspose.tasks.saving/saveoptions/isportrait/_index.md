---
title: "SaveOptions.IsPortrait"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν η προσανατολισμός της σελίδας είναι πορτραίτο, επιστρέφει false εάν η προσανατολισμός της σελίδας είναι τοπίο"
type: docs
weight: 70
url: /el/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν ο προσανατολισμός της σελίδας είναι πορτραίτο· επιστρέφει false εάν ο προσανατολισμός της σελίδας είναι τοπίο.

```csharp
public bool IsPortrait { get; set; }
```

## Παρατηρήσεις

Δεν ισχύει όταν SaveOptions.PageSize == Visualization.PageSize.DefinedInView. Σε αυτήν την περίπτωση χρησιμοποιείται View.PageInfo.PageSettings.IsPortrait. Δεν ισχύει όταν έχει οριστεί SaveOptions.CustomPageSize.

## Παραδείγματα

Δείχνει πώς να καθορίσετε το μέγεθος και τον προσανατολισμό της σελίδας χρησιμοποιώντας τις ρυθμίσεις View ή χρησιμοποιώντας το SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// Σε αυτήν την περίπτωση το μέγεθος και ο προσανατολισμός της σελίδας εφαρμόζονται από τις ιδιότητες view.PageInfo.PageSettings.PaperSize και view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// Σε αυτήν την περίπτωση το μέγεθος και ο προσανατολισμός της σελίδας εφαρμόζονται από τις ιδιότητες του SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// Σε αυτήν την περίπτωση το μέγεθος της σελίδας εφαρμόζεται από το SaveOptions.CustomPageSize. Η ιδιότητα IsPortrait δεν λαμβάνεται υπόψη.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Δείτε επίσης

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


