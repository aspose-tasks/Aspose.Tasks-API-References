---
title: "Αντιπρόσωπος DateTimeConverter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Αντιπροσωπεύει μια μέθοδο μετατροπέα για τη μετατροπή της ημερομηνίας σε συμβολοσειρά σε επίπεδα κλίμακας χρόνου προβολής"
type: docs
weight: 2990
url: /el/net/aspose.tasks.visualization/datetimeconverter/
---
## DateTimeConverter delegate

Αναπαριστά μια μέθοδο μετατροπέα για τη μετατροπή της ημερομηνίας σε συμβολοσειρά σε επίπεδα κλίμακας χρόνου προβολής.

```csharp
public delegate string DateTimeConverter(DateTime date);
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερομηνία | DateTime | η παρουσία της κλάσης DateTime για μετατροπή σε συμβολοσειρά. |

### Τιμή Επιστροφής

η συμβολοσειρά αναπαράστασης της καθορισμένης ημερομηνίας.

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


