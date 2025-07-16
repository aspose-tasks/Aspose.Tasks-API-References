---
title: Class ViewCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ViewCollection class. Contains a list of View objects. Implements ICollectionView interface
type: docs
weight: 2820
url: /net/aspose.tasks/viewcollection/
---
## ViewCollection class

Contains a list of [`View`](../view/) objects. Implements ICollection&lt;View&gt; interface.

```csharp
public class ViewCollection : ICollection<View>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | Gets the parent of the View object. Read-only [`Project`](../project/). |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | Searches for a View with the name, and returns the first occurrence within the collection. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | Searches for a View with the specified Screen property, and returns the first occurrence within the collection. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | Removes the first occurrence of a specific object from this collection. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | Converts a view collection to a list of [`View`](../view/) objects. |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


