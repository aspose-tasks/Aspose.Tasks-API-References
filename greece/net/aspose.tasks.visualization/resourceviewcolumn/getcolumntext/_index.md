---
title: "ResourceViewColumn.GetColumnText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceViewColumn. Μετατρέπει τον τρέχοντα πόρο σε κείμενο στήλης"
type: docs
weight: 30
url: /el/net/aspose.tasks.visualization/resourceviewcolumn/getcolumntext/
---
## ResourceViewColumn.GetColumnText method

Μετατρέπει τον τρέχοντα πόρο σε κείμενο στήλης.

```csharp
public string GetColumnText(Resource resource)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πόρος | Πόρος | Τρέχων πόρος. |

### Τιμή Επιστροφής

Το κείμενο στήλης.

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

* class [Resource](../../../aspose.tasks/resource/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


