---
title: "View.VisualObjectsPlacements"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство View. Возвращает коллекцию объектов, представляющих размещение и внешний вид OleObject в представлении."
type: docs
weight: 130
url: /ru/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

Возвращает коллекцию объектов, представляющих размещение и внешний вид [`OleObject`](../../oleobject/) в представлении.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## Примеры

Показывает, как получить свойства размещения и внешнего вида объекта OLE.

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

### См. также

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


