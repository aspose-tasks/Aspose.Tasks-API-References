---
title: ViewCollection.Contains
second_title: Aspose.Tasks for .NET API Reference
description: ViewCollection method. Returns true if the specified item is found in this collection otherwise false
type: docs
weight: 60
url: /net/aspose.tasks/viewcollection/contains/
---
## ViewCollection.Contains method

Returns true if the specified item is found in this collection; otherwise, false.

```csharp
public bool Contains(View item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | View | the specified item to find. |

### Return Value

true if the specified item is found in this collection; otherwise, false.

## Examples

Shows how to work with view collections.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// convert to a plain list of views
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// add a new view
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// iterate over views
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// remove all views at once
project.Views.Clear();

// or one by one
{
    // approach 1
    List<View> listToDelete = project.Views.ToList();
    foreach (var v in listToDelete)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}

{
    // approach 2
    var array = new View[project.Views.Count];
    project.Views.CopyTo(array, 0);
    foreach (var v in array)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}
```

### See Also

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


