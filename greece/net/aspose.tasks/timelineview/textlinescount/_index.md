---
title: "TimelineView.TextLinesCount"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα TimelineView. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει πόσες γραμμές χρησιμοποιούνται για την εμφάνιση εργασίας σε χρονοδιάγραμμα"
type: docs
weight: 80
url: /el/net/aspose.tasks/timelineview/textlinescount/
---
## TimelineView.TextLinesCount property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει πόσες γραμμές χρησιμοποιούνται για την εμφάνιση εργασιών σε ένα χρονολόγιο.

```csharp
public int TextLinesCount { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με &lt;see cref="Aspose.Tasks.TimelineView" /&gt;.

```csharp
var project = new Project();

// αρχικοποιήστε μια προβολή χρονολογίου
var view = new TimelineView();

// ορίστε μια τιμή που υποδεικνύει πώς να μορφοποιηθούν οι ημερομηνίες στην προβολή Timeline.
view.DateFormat = DateFormat.DateDddDd;
// ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζονται επικαλυπτόμενες εργασίες σε πολλές γραμμές.
view.DisplayOverlapped = true;
// ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζεται ο έλεγχος μετακίνησης και ζουμ.
view.ShowPanZoom = true;
// ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζεται η κλίμακα χρόνου.
view.ShowTimescale = true;
// ορίστε μια τιμή που υποδεικνύει εάν θα εμφανίζεται μια γραμμή που αντιπροσωπεύει τη σημερινή ημέρα.
view.ShowToday = true;
// ορίστε μια τιμή που υποδεικνύει πόσες γραμμές χρησιμοποιούνται για την εμφάνιση εργασιών σε ένα χρονολόγιο.
view.TextLinesCount = 2;

// λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζονται επικαλυπτόμενες εργασίες σε πολλές γραμμές.
Console.WriteLine("Show Dates: " + view.ShowDates);

// προσθέστε την προβολή στο έργο
project.Views.Add(view);

// προσθέστε κάποια δεδομένα δοκιμής στο έργο
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### Δείτε επίσης

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


