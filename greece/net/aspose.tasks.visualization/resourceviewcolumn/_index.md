---
title: "Κλάση ResourceViewColumn"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.ResourceViewColumn κλάση. Κλάση προβολής έργων που χρησιμοποιείται στην προβολή ResourceUsage και στην προβολή ResourceSheet."
type: docs
weight: 3350
url: /el/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

Κλάση προβολής του έργου που χρησιμοποιείται στην προβολή ResourceUsage και στην προβολή ResourceSheet.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `ResourceViewColumn`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | Πεδίο στήλης. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Λαμβάνει το όνομα της στήλης. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Λαμβάνει ή ορίζει την ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της απαρίθμησης [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Λαμβάνει ή ορίζει την κλήση επιστροφής (callback) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης των κελιών της στήλης. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Λαμβάνει το πλάτος της στήλης. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | Μετατρέπει τον τρέχοντα πόρο σε κείμενο στήλης. |

## Παραδείγματα

Δείχνει πώς να προσθέσετε στήλες προβολής πόρων για εξαγωγή.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// επανάληψη στις στήλες
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### Δείτε επίσης

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


