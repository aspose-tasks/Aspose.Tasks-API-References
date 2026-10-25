---
title: "Κλάση View"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.View κλάση. Αντιπροσωπεύει μια προβολή στο Project"
type: docs
weight: 2890
url: /el/net/aspose.tasks/view/
---
## View class

Αντιπροσωπεύει μια προβολή στο Project.

```csharp
public class View : IComparable<View>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [View](view/#constructor)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `View`. |
| [View](view/#constructor_1)(ViewScreen) | Αρχικοποιεί μια νέα παρουσία της κλάσης `View`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Λαμβάνει ή ορίζει ένα φίλτρο που χρησιμοποιείται σε μια μοναδική προβολή. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Λαμβάνει ή ορίζει μια ομάδα της μοναδικής προβολής. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το Microsoft Project επισημαίνει το φίλτρο για μια μοναδική προβολή. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Λαμβάνει ή ορίζει το όνομα ενός αντικειμένου View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Λαμβάνει μια παρουσία της κλάσης [`PageInfo`](./pageinfo/). Αντιπροσωπεύει δεδομένα ρύθμισης σελίδας που υπάρχουν σε μορφή αρχείου mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Λαμβάνει το γονέα του αντικειμένου View. Μόνο για ανάγνωση [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Λαμβάνει τον τύπο οθόνης για τη μοναδική προβολή. Μόνο για ανάγνωση [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το Microsoft Project εμφανίζει το όνομα της μοναδικής προβολής στη λίστα προβολών View ή Other Views στο Ribbon. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Λαμβάνει ή ορίζει έναν πίνακα της μοναδικής προβολής. |
| [Type](../../aspose.tasks/view/type/) { get; } | Λαμβάνει τον τύπο του στοιχείου στη μοναδική προβολή, όπως εργασίες ή πόρους. Μόνο για ανάγνωση [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Λαμβάνει το μοναδικό αναγνωριστικό μιας προβολής. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Λαμβάνει μια συλλογή αντικειμένων που αντιπροσωπεύουν τη θέση και την εμφάνιση του [`OleObject`](../oleobject/) στην προβολή. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Συγκρίνει την τρέχουσα παρουσία με ένα άλλο αντικείμενο του ίδιου τύπου και επιστρέφει έναν ακέραιο που υποδεικνύει εάν η τρέχουσα παρουσία προηγείται, ακολουθεί ή βρίσκεται στην ίδια θέση στη σειρά ταξινόμησης όπως το άλλο αντικείμενο. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης [`Resource`](../resource/). |
| [operator ==](../../aspose.tasks/view/op_equality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο. |

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


