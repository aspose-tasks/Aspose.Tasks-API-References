---
title: "Κλάση TableField"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.TableField κλάση. Αντιπροσωπεύει ένα πεδίο πίνακα σε ένα έργο"
type: docs
weight: 2340
url: /el/net/aspose.tasks/tablefield/
---
## TableField class

Αντιπροσωπεύει ένα πεδίο πίνακα σε ένα έργο.

```csharp
public class TableField
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [TableField](tablefield/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `TableField`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | Λαμβάνει ή ορίζει την ευθυγράμμιση των δεδομένων σε ένα πεδίο πίνακα. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | Λαμβάνει ή ορίζει την ευθυγράμμιση του τίτλου σε ένα πεδίο πίνακα. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο ενός πεδίου πίνακα. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | Λαμβάνει ή ορίζει τον τίτλο του πεδίου σε έναν πίνακα. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | Λαμβάνει ή ορίζει το πλάτος σε σημεία της στήλης πεδίου σε έναν πίνακα. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η επικεφαλίδα στήλης του πίνακα μπορεί να αναδιπλωθεί σε πολλές γραμμές, ή αν πρέπει να περικοπεί όταν υπερβαίνει το πλάτος της στήλης. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το κείμενο της στήλης μπορεί να αναδιπλώνεται σε πολλές γραμμές ή εάν πρέπει να περικόπτεται όταν υπερβαίνει το πλάτος της στήλης. Υποστηρίζεται από την έκδοση MSP 2010 και μεταγενέστερες. |

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

Δείχνει πώς να διαβάσετε τους πίνακες του έργου.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// λάβετε τον πίνακα
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// εμφανίστε όλες τις πληροφορίες των πεδίων του πίνακα
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


