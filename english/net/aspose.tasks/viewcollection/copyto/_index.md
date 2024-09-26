---
title: ViewCollection.CopyTo
second_title: Aspose.Tasks for .NET API Reference
description: ViewCollection method. Copies the elements of this collection to the specified array starting at the specified array index
type: docs
weight: 70
url: /net/aspose.tasks/viewcollection/copyto/
---
## ViewCollection.CopyTo method

Copies the elements of this collection to the specified array, starting at the specified array index.

```csharp
public void CopyTo(View[] array, int arrayIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| array | View[] | the specified one-dimensional array to copy elements to |
| arrayIndex | Int32 | the zero-based index of the specified array at which copying begins. |

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


