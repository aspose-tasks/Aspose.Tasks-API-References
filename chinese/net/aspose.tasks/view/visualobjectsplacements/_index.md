---
title: "View.VisualObjectsPlacements"
second_title: "Aspose.Tasks for .NET API 参考"
description: "View 属性。获取一个对象集合，表示视图中 OleObject 的放置和外观"
type: docs
weight: 130
url: /zh/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

获取一个对象集合，表示视图中 [`OleObject`](../../oleobject/) 的放置和外观。

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## 示例

展示如何获取 OLE 对象的放置和外观属性。

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

### 另见

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


