---
title: "View.VisualObjectsPlacements"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété View. Obtient une collection d’objets représentant le placement et l’apparence de OleObject dans la vue."
type: docs
weight: 130
url: /fr/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

Obtient une collection d’objets représentant le placement et l’apparence de [`OleObject`](../../oleobject/) dans la vue.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## Exemples

Montre comment obtenir les propriétés de placement et d’apparence de l’objet OLE.

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

### Voir aussi

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


