---
title: "Απαρίθμηση TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.Visualization.TimescaleFitBehavior. Αντιπροσωπεύει μια συμπεριφορά που χρησιμοποιείται για την ευθυγράμμιση της περιοχής κλίμακας χρόνου με το πλάτος της σελίδας"
type: docs
weight: 3440
url: /el/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Αντιπροσωπεύει μια συμπεριφορά που χρησιμοποιείται για την ευθυγράμμιση της περιοχής κλίμακας χρόνου με το πλάτος της σελίδας.

```csharp
public enum TimescaleFitBehavior
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| DefinedInView | `0` | Η ενότητα ημερολογίου αποδίδεται σύμφωνα με την ιδιότητα View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage της αποδοθείσας Προβολής. |
| NoScaleToEndDate | `1` | Η ενότητα ημερολογίου αποδίδεται ακριβώς μέχρι την EndDate, ακόμη και αν υπάρχει κενός χώρος σε μια σελίδα. |
| NoScaleToEndOfPage | `2` | Η ενότητα ημερολογίου αποδίδεται μέχρι το τέλος (δεξιά πλευρά) της τελευταίας σελίδας. Συνεπώς η τελευταία αποδοθείσα ημερομηνία μπορεί να υπερβαίνει την EndDate. |
| ScaleToEndOfPage | `3` | Η μηχανή απόδοσης θα προσπαθήσει να ευθυγραμμίσει τις ημερομηνίες ώστε η EndDate να ευθυγραμμίζεται με το τέλος (δεξιά πλευρά) της τελευταίας σελίδας. Συμφωνεί με την ενεργοποιημένη επιλογή "Page Setup \ View \ Fit timescale to end of page" του MS Project. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε το TimescaleFitBehavior για να κάνετε την κλίμακα χρόνου του διαγράμματος Gantt να ταιριάζει στο τέλος της τελευταίας σελίδας.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


