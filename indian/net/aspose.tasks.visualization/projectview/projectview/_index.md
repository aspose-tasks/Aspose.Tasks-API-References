---
title: "ProjectView.ProjectView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectView कंस्ट्रक्टर। ProjectView क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.visualization/projectview/projectview/
---
## ProjectView constructor

एक नया इंस्टेंस इनिशियलाइज़ करता है [`ProjectView`](../) क्लास का।

```csharp
public ProjectView(IEnumerable<ViewColumn> columns)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कॉलम | IEnumerable`1 | दृश्य कॉलमों की एक सूची। |

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


