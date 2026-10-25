---
title: "GanttBarStyle.ShowForCategories"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttBarStyle प्रॉपर्टी। उन टास्क श्रेणियों को प्राप्त करता है या सेट करता है जिनके लिए शैली लागू होती है। यह गैंट चार्ट में बार की पैरेंट या सामान्य शैलियों के लिए लागू होती है, देखें BarStyles।"
type: docs
weight: 200
url: /hi/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

शैली के लागू होने वाले टास्क श्रेणियों को प्राप्त करता है या सेट करता है। यह गैंट चार्ट में बार की पैरेंट (या सामान्य) शैलियों के लिए लागू होती है (देखें [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/))।

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
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

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


