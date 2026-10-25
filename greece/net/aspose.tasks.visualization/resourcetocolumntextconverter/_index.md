---
title: "Διαμεσολαβητής ResourceToColumnTextConverter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μετατροπέας δεδομένων πόρων σε συμβολοσειρά στηλών"
type: docs
weight: 3340
url: /el/net/aspose.tasks.visualization/resourcetocolumntextconverter/
---
## ResourceToColumnTextConverter delegate

Μετατροπέας δεδομένων πόρων σε συμβολοσειρά στήλης.

```csharp
public delegate string ResourceToColumnTextConverter(Resource resource);
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πόρος | Πόρος | Τρέχων πόρος. |

### Τιμή Επιστροφής

Συμβολοσειρά δεδομένων για τη στήλη.

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

* class [Resource](../../aspose.tasks/resource/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


