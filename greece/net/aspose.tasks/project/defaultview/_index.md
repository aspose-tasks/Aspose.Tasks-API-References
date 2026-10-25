---
title: "Project.DefaultView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει ή ορίζει την προεπιλεγμένη προβολή του έργου"
type: docs
weight: 360
url: /el/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

Αποκτά ή ορίζει την προεπιλεγμένη προβολή του έργου.

```csharp
public View DefaultView { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με την προεπιλεγμένη προβολή ενός έργου.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// Λάβετε προεπιλεγμένη προβολή
UsageView view = (TaskUsageView)project.DefaultView;

// Η στήλη κεφαλίδας λεπτομερειών δεν θα εμφανιστεί
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// Εμφάνιση στήλης κεφαλίδας λεπτομερειών
view.DisplayDetailsHeaderColumn = true;

// Επανάληψη κεφαλίδας λεπτομερειών σε όλες τις γραμμές αναθέσεων
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

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

### Δείτε επίσης

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


