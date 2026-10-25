---
title: "Enum TimescaleUnit"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.TimescaleUnit enum. Καθορίζει τη μονάδα χρόνου για οποιοδήποτε επίπεδο μιας κλίμακας χρόνου σε διάγραμμα Gantt ή άλλη προβολή φάσης χρόνου."
type: docs
weight: 3460
url: /el/net/aspose.tasks.visualization/timescaleunit/
---
## TimescaleUnit enumeration

Καθορίζει τη μονάδα χρόνου για οποιοδήποτε επίπεδο κλίμακας χρόνου σε διάγραμμα Gantt ή άλλη προβολή φάσης χρόνου.

```csharp
public enum TimescaleUnit
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `-1` | Δείχνει Καμία. Το επίπεδο της κλίμακας χρόνου είναι κρυφό. |
| Minutes | `0` | Δείχνει τη μονάδα κλίμακας χρόνου Λεπτά. |
| Hours | `1` | Δείχνει τη μονάδα κλίμακας χρόνου Ώρες. |
| Days | `2` | Δείχνει τη μονάδα κλίμακας χρόνου Ημέρες. |
| Weeks | `3` | Δείχνει τη μονάδα κλίμακας χρόνου Εβδομάδες. |
| ThirdsOfMonths | `4` | Δείχνει τη μονάδα κλίμακας χρόνου Τρίτα του μήνα. |
| Months | `5` | Δείχνει τη μονάδα κλίμακας χρόνου Μήνες. |
| Quarters | `6` | Δείχνει τη μονάδα κλίμακας χρόνου Τρίμηνα του έτους. |
| HalfYears | `7` | Δείχνει τη μονάδα κλίμακας χρόνου Μισό έτος. |
| Years | `8` | Δείχνει τη μονάδα κλίμακας χρόνου Έτη. |

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


