---
title: ResourceViewColumn.GetColumnText
second_title: Aspose.Tasks for .NET API Reference
description: ResourceViewColumn method. Converts current resource to the column text
type: docs
weight: 30
url: /net/aspose.tasks.visualization/resourceviewcolumn/getcolumntext/
---
## ResourceViewColumn.GetColumnText method

Converts current resource to the column text.

```csharp
public string GetColumnText(Resource resource)
```

| Parameter | Type | Description |
| --- | --- | --- |
| resource | Resource | Current resource. |

### Return Value

The column text.

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

* class [Resource](../../../aspose.tasks/resource/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


