---
title: View.VisualObjectsPlacements
second_title: Aspose.Tasks for .NET API Reference
description: View property. Gets a collection of objects representing placement and appearance of OleObject in the view
type: docs
weight: 130
url: /net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

Gets a collection of objects representing placement and appearance of [`OleObject`](../../oleobject/) in the view.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## Examples

Shows how to get OLE object's placement and appearance properties.

```csharp
[Test]
public void GetVisualObjectPlacementProperties()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    var oleObject = project.OleObjects.First();

    project.Save(OutDir + "ClearedProject.mpp");
    var view = project.Views.First(v => v.Name == "&Gantt Chart");
    var oleObjectPlacement = view.VisualObjectsPlacements.First(p => p.OleObjectId == oleObject.Id);

    Console.WriteLine("BorderLineColor: {0}", oleObjectPlacement.BorderLineColor);
    Console.WriteLine("BorderLineColor: {0}", oleObjectPlacement.BorderLineThickness);

    if (oleObjectPlacement.TaskId > 0)
    {
        Console.WriteLine("Attached to task: {0}", oleObjectPlacement.TaskId);
    }
    else
    {
        Console.WriteLine("Attached to timescale date: {0}", oleObjectPlacement.TimescaleDate);
    }
}
```

### See Also

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


