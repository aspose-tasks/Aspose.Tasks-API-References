---
title: "View.VisualObjectsPlacements"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti View. Mengambil koleksi objek yang mewakili penempatan dan tampilan OleObject dalam tampilan."
type: docs
weight: 130
url: /id/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

Mengambil koleksi objek yang mewakili penempatan dan tampilan [`OleObject`](../../oleobject/) dalam tampilan.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## Contoh

Menampilkan cara mendapatkan properti penempatan dan tampilan objek OLE.

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

### Lihat Juga

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


