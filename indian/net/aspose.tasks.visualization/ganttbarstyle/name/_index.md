---
title: "GanttBarStyle.Name"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttBarStyle गुण। शैली का नाम प्राप्त करता है या सेट करता है"
type: docs
weight: 150
url: /hi/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

स्टाइल का नाम प्राप्त करता है या सेट करता है।

```csharp
public string Name { get; set; }
```

## उदाहरण

ShowFor श्रेणियों के उपयोग को दर्शाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");
var view = (GanttChartView)project.DefaultView;

var barStyle = this.GetCustomBarStyle();
barStyle.ShowForTaskUid = null;

var showForCategories = new[]
{
    GanttBarShowFor.Active,
    GanttBarShowFor.NotSummary,
    GanttBarShowFor.Milestone,
    GanttBarShowFor.Finished
};

barStyle.ShowForCategories = new List<GanttBarShowFor>(showForCategories);
barStyle.Name = "My common style";
view.BarStyles.Add(barStyle);

// परियोजना के साथ काम करें...
```

### संबंधित देखें

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


