---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectView मेथड। इसमें id संकेतक, नाम, अवधि, प्रारंभ, समाप्ति, पूर्ववर्ती और संसाधन नाम कार्य कॉलम शामिल हैं"
type: docs
weight: 60
url: /hi/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

id, indicators, name, duration, start, finish, predecessors और resource names टास्क कॉलम शामिल हैं।

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### रिटर्न वैल्यू

एक दृश्य जिसमें [`GanttChartColumn`](../../ganttchartcolumn/) की सूची शामिल है।

## उदाहरण

दिखाता है कि टास्क शीट दृश्य के साथ प्रोजेक्ट को कैसे सहेजें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### संबंधित देखें

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


