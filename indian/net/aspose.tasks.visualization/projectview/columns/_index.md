---
title: "ProjectView.Columns"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectView प्रॉपर्टी। प्रोजेक्ट व्यू कॉलम प्राप्त करता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks.visualization/projectview/columns/
---
## ProjectView.Columns property

प्रोजेक्ट व्यू कॉलम प्राप्त करता है।

```csharp
public List<ViewColumn> Columns { get; }
```

## उदाहरण

दिखाता है कि कस्टम कॉलम सेट वाले दृश्य के साथ प्रोजेक्ट को कैसे सहेजें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new GanttChartColumn("Name", 100, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("Finish", 100, Field.TaskFinish),
    new GanttChartColumn("Cost2", 80, Field.TaskCost2),
    new GanttChartColumn("Number6", 80, Field.TaskNumber6),
    new GanttChartColumn("Date6", 80, Field.TaskDate6),
    new GanttChartColumn("Flag6", 80, Field.TaskFlag6),
    new GanttChartColumn("Flag18", 80, Field.TaskFlag18),
    new GanttChartColumn("Duration6", 80, Field.TaskDuration6)
};
options.View = new ProjectView(columns);

// दृश्य कॉलमों पर इटररेट करें
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### संबंधित देखें

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


