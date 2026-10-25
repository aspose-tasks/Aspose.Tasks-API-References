---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttBarStyle गुण। उस कार्य का यूनिक आईडी प्राप्त करता है या सेट करता है जिसके लिए शैली लागू होती है। गैंट चार्ट में बार की कार्य-विशिष्ट शैलियों के लिए लागू है, देखें CustomBarStyles"
type: docs
weight: 210
url: /hi/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

उस कार्य का यूनिक आईडी प्राप्त करता है या सेट करता है जिसके लिए शैली लागू होती है। गैंट चार्ट में बार की कार्य-विशिष्ट शैलियों के लिए लागू है (देखें [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
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


