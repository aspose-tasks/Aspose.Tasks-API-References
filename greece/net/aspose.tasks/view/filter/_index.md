---
title: "View.Filter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "View property. Λαμβάνει ή ορίζει ένα φίλτρο που χρησιμοποιείται σε μια μοναδική προβολή"
type: docs
weight: 20
url: /el/net/aspose.tasks/view/filter/
---
## View.Filter property

Λαμβάνει ή ορίζει ένα φίλτρο που χρησιμοποιείται σε μια μοναδική προβολή.

```csharp
public Filter Filter { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις προβολές του MS Project.

```csharp
// Δημιουργήστε ένα κενό έργο χωρίς προβολές
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// δημιουργήστε μια τυπική προβολή διαγράμματος Gantt
View view = new GanttChartView();

// ορίστε ορισμένες ιδιότητες προβολής
// ορίστε μια τιμή που υποδεικνύει εάν το Microsoft Project εμφανίζει το όνομα της μοναδικής προβολής στη λίστα View ή Other Views στη Ribbon
view.ShowInMenu = true;
// ορίστε μια τιμή που υποδεικνύει εάν το Microsoft Project επισημαίνει το φίλτρο για μια μοναδική προβολή
view.HighlightFilter = true;

// η εγγραφή των επόμενων ιδιοτήτων δεν υποστηρίζεται
// ορίζει το φίλτρο που χρησιμοποιείται σε μια μοναδική προβολή
view.Filter = null;
// ορίζει την ομάδα της μοναδικής προβολής
view.Group = null;
// ορίζει τον πίνακα της μοναδικής προβολής
view.Table = null;

// ας ρυθμίσουμε ορισμένες ρυθμίσεις προβολής
// ορίστε τον αριθμό των πρώτων στηλών που θα εκτυπωθούν σε όλες τις σελίδες
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// ορίστε μια τιμή που υποδεικνύει εάν θα εκτυπωθεί καθορισμένος αριθμός πρώτων στηλών σε όλες τις σελίδες
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// προσθέστε την προβολή στο έργο μας
project.Views.Add(view);

// Η σημαία WriteViewData πρέπει να χρησιμοποιηθεί για τη διατήρηση των project.Views.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// ας ελέγξουμε ορισμένες ιδιότητες της πρόσφατα προστιθέμενης προβολής
// εκτυπώστε το μοναδικό αναγνωριστικό μιας προβολής
Console.WriteLine("View Uid: " + view.Uid);
// εκτυπώστε τον τύπο οθόνης για τη μοναδική προβολή
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### Δείτε επίσης

* class [Filter](../../filter/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


