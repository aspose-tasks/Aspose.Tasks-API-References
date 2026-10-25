---
title: "View.VisualObjectsPlacements"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "View-eigenschap. Haalt een collectie objecten op die de plaatsing en weergave van OleObject in de weergave vertegenwoordigen."
type: docs
weight: 130
url: /nl/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

Haalt een collectie objecten op die de plaatsing en weergave van [`OleObject`](../../oleobject/) in de weergave.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## Voorbeelden

Toont hoe de plaatsings- en weergave-eigenschappen van een OLE-object op te halen.

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

### Zie ook

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


