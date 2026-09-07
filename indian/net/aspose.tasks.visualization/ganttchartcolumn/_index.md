---
title: "क्लास GanttChartColumn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.GanttChartColumn क्लास। प्रोजेक्ट्स व्यू क्लास"
type: docs
weight: 3090
url: /hi/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

प्रोजेक्ट का दृश्य वर्ग

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | कॉलम फ़ील्ड। [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | कॉलम का नाम प्राप्त करता है। |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | पाठ की संरेखण प्राप्त करता है या सेट करता है (यह [`HorizontalStringAlignment`](../horizontalstringalignment/) enumeration के मानों में से एक हो सकता है)। |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | कॉलम की कोशिकाओं की उपस्थिति को अनुकूलित करने के लिए उपयोग की जा सकने वाली कॉलबैक प्राप्त करता है या सेट करता है। |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | कॉलम की चौड़ाई प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | वर्तमान कार्य को कॉलम टेक्स्ट में बदलता है। |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


