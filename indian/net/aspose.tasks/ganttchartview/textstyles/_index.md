---
title: "GanttChartView.TextStyles"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttChartView प्रॉपर्टी। Gantt Chart दृश्य की TextStyle की सूची प्राप्त करता है या सेट करता है"
type: docs
weight: 170
url: /hi/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Gantt Chart दृश्य की [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) की सूची प्राप्त करता है या सेट करता है।

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## उदाहरण

दिखाता है कि Gantt चार्ट टेक्स्ट स्टाइल कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// Gantt चार्ट दृश्य के टेक्स्ट स्टाइल पर इटररेट करें
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### संबंधित देखें

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


