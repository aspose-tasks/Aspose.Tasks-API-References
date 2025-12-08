---
title: Class ResourceViewColumn
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.ResourceViewColumn class. Projects view class used in ResourceUsage view and ResourceSheet view
type: docs
weight: 3300
url: /net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

Project's view class used in ResourceUsage view and ResourceSheet view.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## Constructors

| Name | Description |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | Initializes a new instance of the `ResourceViewColumn` class. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | Initializes a new instance of the `ResourceViewColumn` class. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | Initializes a new instance of the `ResourceViewColumn` class. |

## Properties

| Name | Description |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | Column field. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Gets the column name. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Gets or sets alignment of the text (can be one of the values of the [`HorizontalStringAlignment`](../horizontalstringalignment/) enumeration). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Gets or sets the callback which can be used to customize the appearance of the column's cells. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Gets the column width. |

## Methods

| Name | Description |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | Converts current resource to the column text. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


