---
title: "View.VisualObjectsPlacements"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية View. تُجلب مجموعة من الكائنات التي تمثل موضع ومظهر OleObject في العرض"
type: docs
weight: 130
url: /ar/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

تُجلب مجموعة من الكائنات التي تمثل موضع ومظهر [`OleObject`](../../oleobject/) في العرض.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## الأمثلة

يُظهر كيفية الحصول على خصائص موضع ومظهر كائن OLE.

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

### انظر أيضًا

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


