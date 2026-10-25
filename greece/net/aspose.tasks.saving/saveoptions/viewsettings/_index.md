---
title: "SaveOptions.ViewSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια προβολή View για απόδοση. Μπορείτε να χρησιμοποιήσετε αυτήν την επιλογή για να καθορίσετε ρητά ποια προβολή πρέπει να αποθηκευτεί σε μορφές PDF, HTML ή Image. Εάν αυτή η ιδιότητα οριστεί, η ιδιότητα PresentationFormat αγνοείται όταν αποθηκεύεται το έργο. Η προβολή πρέπει να προέρχεται από μία από τις ακόλουθες οθόνες Screen Gantt TaskSheet TaskUsage ResourceSheet ResourceUsage."
type: docs
weight: 240
url: /el/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Λαμβάνει ή ορίζει μια προβολή ([`View`](../view/)) για απόδοση. Μπορείτε να χρησιμοποιήσετε αυτήν την επιλογή για να καθορίσετε ρητά ποια προβολή πρέπει να αποθηκευτεί σε μορφές PDF, HTML ή Image. Εάν αυτή η ιδιότητα οριστεί, η ιδιότητα [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) αγνοείται όταν αποθηκεύεται το έργο. Η προβολή πρέπει να προέρχεται από μία από τις ακόλουθες οθόνες (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

```csharp
public View ViewSettings { get; set; }
```

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Όταν καλείται η μέθοδος set και παρέχεται ένα αντικείμενο της κλάσης View με μη υποστηριζόμενη τιμή της ιδιότητας Screen. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε το 'SaveOptions.ViewSettings' για να καθορίσετε την προβολή που πρέπει να αποδοθεί σε PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### Δείτε επίσης

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


