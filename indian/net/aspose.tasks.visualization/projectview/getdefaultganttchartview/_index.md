---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectView मेथड। इसमें id संकेतक, नाम, अवधि, प्रारंभ और समाप्ति कार्य कॉलम शामिल हैं"
type: docs
weight: 30
url: /hi/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

id, संकेतक, नाम, अवधि, प्रारंभ और समाप्ति कार्य कॉलम शामिल करता है।

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### रिटर्न वैल्यू

एक दृश्य जिसमें [`GanttChartColumn`](../../ganttchartcolumn/) की सूची शामिल है।

## उदाहरण

दिखाता है कि Gantt चार्ट दृश्य के साथ प्रोजेक्ट को कैसे सहेजें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### संबंधित देखें

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


