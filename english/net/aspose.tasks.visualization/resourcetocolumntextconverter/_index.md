---
title: Delegate ResourceToColumnTextConverter
second_title: Aspose.Tasks for .NET API Reference
description: Resources data to columns string converter
type: docs
weight: 3290
url: /net/aspose.tasks.visualization/resourcetocolumntextconverter/
---
## ResourceToColumnTextConverter delegate

Resource's data to column's string converter.

```csharp
public delegate string ResourceToColumnTextConverter(Resource resource);
```

| Parameter | Type | Description |
| --- | --- | --- |
| resource | Resource | Current resource. |

### Return Value

String data for the column.

## Examples

Shows how to add resource view columns to be exported.

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

// iterate over columns
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

### See Also

* class [Resource](../../aspose.tasks/resource/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


