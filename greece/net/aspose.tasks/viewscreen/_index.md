---
title: "Απαρίθμηση ViewScreen"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.ViewScreen. Καθορίζει τον τύπο οθόνης για μια προβολή"
type: docs
weight: 2910
url: /el/net/aspose.tasks/viewscreen/
---
## ViewScreen enumeration

Καθορίζει τον τύπο οθόνης για μια προβολή.

```csharp
public enum ViewScreen
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Calendar | `13` | Προβολή Ημερολογίου. |
| Gantt | `1` | Προβολή Gantt. |
| NetworkDiagram | `2` | Προβολή Διαγράμματος Δικτύου. |
| RelationshipDiagram | `3` | Προβολή Διαγράμματος Σχέσεων. |
| ResourceForm | `6` | Προβολή Φόρμας Πόρων. |
| ResourceGraph | `8` | Προβολή Γραφήματος Πόρων. |
| ResourceNameForm | `12` | Προβολή Φόρμας Ονόματος Πόρου. |
| ResourceSheet | `7` | Προβολή Φύλλου Πόρων. |
| ResourceUsage | `15` | Προβολή Χρήσης Πόρων. |
| TaskDetailsForm | `10` | Προβολή Φόρμας Λεπτομερειών Εργασίας. |
| TaskForm | `4` | Προβολή Φόρμας Εργασίας. |
| TaskNameForm | `11` | Προβολή Φόρμας Ονόματος Εργασίας. |
| TaskSheet | `5` | Προβολή Φύλλου Εργασίας. |
| TaskUsage | `14` | Προβολή Χρήσης Εργασίας. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με την προβολή του Project και να προσθέσετε στήλη στην προεπιλεγμένη προβολή (η οποία εμφανίζεται όταν ανοίγεται αρχείο MPP στο MS Project).

```csharp
// Δημιουργήστε ένα κενό έργο χωρίς προβολές
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Τροποποιήστε την προεπιλεγμένη προβολή (είναι προβολή διαγράμματος Gantt).
// Ή μπορείτε να επιλέξετε προβολή κατά όνομα ή μέσω της οθόνης προβολής χρησιμοποιώντας τη συλλογή project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Η σημαία WriteViewData πρέπει να χρησιμοποιείται για τη διατήρηση των τροποποιήσεων των ιδιοτήτων της προβολής.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


