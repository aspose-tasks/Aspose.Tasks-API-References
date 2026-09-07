---
title: "डेलीगेट TaskToColumnTextConverter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "टास्क डेटा को कॉलम स्ट्रिंग में बदलने वाला कनवर्टर"
type: docs
weight: 3400
url: /hi/net/aspose.tasks.visualization/tasktocolumntextconverter/
---
## TaskToColumnTextConverter delegate

टास्क डेटा को कॉलम की स्ट्रिंग में बदलने वाला कनवर्टर।

```csharp
public delegate string TaskToColumnTextConverter(Task task);
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कार्य | कार्य | वर्तमान कार्य। |

### रिटर्न वैल्यू

कॉलम के लिए स्ट्रिंग डेटा।

## उदाहरण

दिखाता है कि निर्यात करने के लिए Gantt चार्ट व्यू कॉलम कैसे जोड़ें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.GetById(1);

var columns = new List<ViewColumn>
{
    new GanttChartColumn(20, Field.TaskUniqueID),
    new GanttChartColumn("Name", 150, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("End", 100, Field.TaskFinish),
    new GanttChartColumn("R-Initials", 100, Field.TaskResourceInitials),
    new GanttChartColumn("R-Names", 100, Field.TaskResourceNames),
    new GanttChartColumn("Work", 50, Field.TaskWork),
    new GanttChartColumn(
        "Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new GanttChartColumn(
        "Actual Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.ActualCost).ToString(CultureInfo.InvariantCulture);
        },
        Field.TaskActualCost)
};

// कॉलम पर इटररेट करें
foreach (var column in columns)
{
    var col = (GanttChartColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(task));
    Console.WriteLine();
}

var options = new CsvOptions
{
    View = new ProjectView(columns)
};

project.Save(OutDir + "WorkWithGanttChartColumn_out.csv", options);
```

### संबंधित देखें

* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


