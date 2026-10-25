---
title: "View.VisualObjectsPlacements"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "View प्रॉपर्टी। OleObject की प्लेसमेंट और उपस्थिति को दर्शाने वाले ऑब्जेक्ट्स का संग्रह प्राप्त करता है।"
type: docs
weight: 130
url: /hi/net/aspose.tasks/view/visualobjectsplacements/
---
## View.VisualObjectsPlacements property

व्यू में [`OleObject`](../../oleobject/) की प्लेसमेंट और उपस्थिति को दर्शाने वाले ऑब्जेक्ट्स का संग्रह प्राप्त करता है।

```csharp
public IEnumerable<VisualObjectPlacement> VisualObjectsPlacements { get; }
```

## उदाहरण

दिखाता है कि OLE ऑब्जेक्ट की प्लेसमेंट और उपस्थिति प्रॉपर्टीज़ कैसे प्राप्त करें।

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

### संबंधित देखें

* class [VisualObjectPlacement](../../../aspose.tasks.visualization/visualobjectplacement/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


