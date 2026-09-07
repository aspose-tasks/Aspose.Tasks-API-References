---
title: "ResourceViewColumn.Field"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ResourceViewColumn. Πεδίο στήλης. Field"
type: docs
weight: 20
url: /el/net/aspose.tasks.visualization/resourceviewcolumn/field/
---
## ResourceViewColumn.Field property

Πεδίο στήλης. `Field`.

```csharp
public override Field Field { get; set; }
```

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

* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


