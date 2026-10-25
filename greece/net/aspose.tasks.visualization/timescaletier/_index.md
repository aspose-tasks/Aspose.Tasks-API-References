---
title: "Κλάση TimescaleTier"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.TimescaleTier κλάση. Αντιπροσωπεύει ένα μοναδικό επίπεδο της κλίμακας χρόνου σε ένα Διάγραμμα Gantt"
type: docs
weight: 3450
url: /el/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Αναπαριστά ένα μοναδικό επίπεδο της κλίμακας χρόνου σε ένα Gantt Chart.

```csharp
public sealed class TimescaleTier
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `TimescaleTier`. |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `TimescaleTier`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | Λαμβάνει ή ορίζει πώς θα ευθυγραμμιστούν οι ετικέτες εντός κάθε χρονικής περιόδου του επιπέδου ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | Λαμβάνει ή ορίζει το διάστημα μονάδας χρόνου στο οποίο θα εμφανίζονται οι ετικέτες για το επίπεδο. Η προεπιλεγμένη τιμή είναι 1. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | Λαμβάνει ή ορίζει μια συνάρτηση callback για τη διαχείριση της απόδοσης του χρονοδείκτη σε αυτό το επίπεδο. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | Λαμβάνει ή ορίζει την ετικέτα ημερομηνίας [`DateLabel`](../datelabel/) για το επίπεδο κλίμακας χρόνου. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | Λαμβάνει ή ορίζει τη σημαία που καθορίζει αν οι ετικέτες ημερομηνίας πρέπει να αποδίδονται σε κάθε σελίδα όταν μια χρονική περίοδος εκτείνεται σε πολλές σελίδες. Εάν η τιμή είναι 'true', όταν η χρονική περίοδος εκτείνεται σε πολλές σελίδες, οι ετικέτες ημερομηνίας για την περίοδο αποδίδονται σε κάθε σελίδα. Εάν η τιμή είναι 'false', η ετικέτα ημερομηνίας αποδίδεται μόνο μία φορά σύμφωνα με την τιμή της ιδιότητας [`Alignment`](./alignment/). |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα εμφανίζονται οι γραμμές σήμανσης που διαχωρίζουν τις χρονικές περιόδους στο επίπεδο. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | Λαμβάνει ή ορίζει τη μονάδα κλίμακας χρόνου [`TimescaleUnit`](../timescaleunit/) για το επίπεδο κλίμακας χρόνου. Η προεπιλεγμένη τιμή είναι [`Days`](../timescaleunit/). |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν οι ετικέτες του επιπέδου θα βασίζονται στο οικονομικό έτος. |

## Παραδείγματα

Δείχνει πώς να προσαρμόσετε τις ετικέτες του επιπέδου κλίμακας χρόνου.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Προσθήκη συνδέσμων εργασιών
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// ρυθμίστε τα επίπεδα κλίμακας χρόνου

// ρυθμίστε το ανώτερο επίπεδο
// ορίστε το ανώτερο επίπεδο κλίμακας χρόνου της προβολής Διάγραμμα Gantt.
view.MiddleTimescaleTier = new TimescaleTier();
// ορίστε τη μονάδα κλίμακας χρόνου <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> για το επίπεδο κλίμακας χρόνου.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// ορίστε το διάστημα μονάδας χρόνου στο οποίο θα εμφανίζονται οι ετικέτες για το επίπεδο.
view.MiddleTimescaleTier.Count = 1;
// ορίστε την ετικέτα ημερομηνίας <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> για το επίπεδο κλίμακας χρόνου.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// ορίστε πώς θα ευθυγραμμιστούν οι ετικέτες εντός κάθε χρονικής περιόδου του επιπέδου (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζονται σημεία σήμανσης που χωρίζουν χρονικές περιόδους στο επίπεδο.
view.MiddleTimescaleTier.ShowTicks = true;
// ορίστε μια τιμή που υποδεικνύει εάν οι ετικέτες του επιπέδου θα βασίζονται στο οικονομικό έτος.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// προστέθηκε για καλύτερη απεικόνιση
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// προσαρμόστε τις ημερομηνίες του μεσαίου επιπέδου
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Χρησιμοποιήστε την επιλογή 'Timescale.DefinedInView' για την απόδοση των κλιμάκων χρόνου χρησιμοποιώντας τις ρυθμίσεις κλίμακας χρόνου που ορίζονται στην προβολή (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


