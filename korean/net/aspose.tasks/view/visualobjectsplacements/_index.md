---
title: "View.VisualObjectsPlacements"
second_title: "Aspose.Tasks for .NET API 참조"
description: "View 속성. 보기에서 OleObject의 배치 및 모양을 나타내는 객체 컬렉션을 가져옵니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

보기에서 [`OleObject`](../../oleobject/)의 배치 및 모양을 나타내는 객체 컬렉션을 가져옵니다.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## 예제

OLE 객체의 배치 및 모양 속성을 가져오는 방법을 보여줍니다.

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

### 또 보기

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


