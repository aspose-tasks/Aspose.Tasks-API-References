---
title: "View.VisualObjectsPlacements"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad View. Obtiene una colección de objetos que representan la ubicación y apariencia de OleObject en la vista."
type: docs
weight: 130
url: /es/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

Obtiene una colección de objetos que representan la ubicación y apariencia de [`OleObject`](../../oleobject/) en la vista.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## Ejemplos

Muestra cómo obtener las propiedades de ubicación y apariencia del objeto OLE.

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

### Ver también

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


