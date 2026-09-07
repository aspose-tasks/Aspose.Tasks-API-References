---
title: "GanttChartColumn.GetColumnText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GanttChartColumn मेथड। वर्तमान टास्क को कॉलम टेक्स्ट में परिवर्तित करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks.visualization/ganttchartcolumn/getcolumntext/
---
## GanttChartColumn.GetColumnText method

वर्तमान कार्य को कॉलम टेक्स्ट में बदलता है।

```csharp
public string GetColumnText(Task task)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कार्य | कार्य | वर्तमान कार्य। |

### रिटर्न वैल्यू

कॉलम टेक्स्ट।

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

* class [Task](../../../aspose.tasks/task/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


