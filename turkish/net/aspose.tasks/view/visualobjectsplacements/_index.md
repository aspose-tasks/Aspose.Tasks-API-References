---
title: "View.VisualObjectsPlacements"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "View özelliği. Görünümde OleObject'in yerleşimini ve görünümünü temsil eden nesneler koleksiyonunu alır."
type: docs
weight: 130
url: /tr/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

Görünümde [`OleObject`](../../oleobject/) yerleşimini ve görünümünü temsil eden nesneler koleksiyonunu alır.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## Örnekler

OLE nesnesinin yerleşim ve görünüm özelliklerini nasıl alacağınızı gösterir.

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

### Ayrıca Bakınız

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


