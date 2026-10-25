---
title: "View.VisualObjectsPlacements"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα View. Λαμβάνει μια συλλογή αντικειμένων που αντιπροσωπεύουν τη θέση και την εμφάνιση του OleObject στην προβολή."
type: docs
weight: 130
url: /el/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

Λαμβάνει μια συλλογή αντικειμένων που αντιπροσωπεύουν τη θέση και την εμφάνιση του [`OleObject`](../../oleobject/) στην προβολή.

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## Παραδείγματα

Δείχνει πώς να λάβετε τις ιδιότητες θέσης και εμφάνισης του αντικειμένου OLE.

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

### Δείτε επίσης

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


