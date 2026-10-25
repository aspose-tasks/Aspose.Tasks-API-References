---
title: "ITextStyleModificationCallback.BeforeTaskTextStyleApplied"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ITextStyleModificationCallback मेथड। निम्नलिखित व्यूज़ में टास्क रो के लिए टेबल सेल रेंडर करने से पहले कॉल किया जाने वाला मेथड: Gantt Chart, Task Sheet, Task Usage"
type: docs
weight: 10
url: /hi/net/aspose.tasks.visualization/itextstylemodificationcallback/beforetasktextstyleapplied/
---
## ITextStyleModificationCallback.BeforeTaskTextStyleApplied method

निम्नलिखित दृश्यों में टास्क पंक्ति के लिए टेबल सेल को रेंडर करने से पहले बुलाई जाने वाली विधि: 'Gantt Chart', 'Task Sheet', 'Task Usage'।

```csharp
public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| args | TaskTextStyleEventArgs | यह [`TaskTextStyleEventArgs`](../../tasktextstyleeventargs/) ऑब्जेक्ट। |

## उदाहरण

दिखाता है कि निर्यात करने के लिए दृश्य कॉलम कैसे जोड़ें।

```csharp
public void WorkWithViewColumn()
{
    var project = new Project(DataDir + "Project2.mpp");

    var options = new PdfSaveOptions();
    var columns = new List<ViewColumn>
    {
        new ResourceViewColumn(100, Field.ResourceName),
        new ResourceViewColumn(100, Field.ResourceActualWork),
        new ResourceViewColumn(100, Field.ResourceCost)
    };

    columns[0].TextStyleModificationCallback = new MyTextStyleCallback();

    // कॉलम पर इटररेट करें
    foreach (var column in columns)
    {
        Console.WriteLine("Column Name: " + column.Name);
        Console.WriteLine("Column Field: " + column.Field);
        Console.WriteLine("Column Width: " + column.Width);
        Console.WriteLine("Column Callback: " + column.TextStyleModificationCallback);
        Console.WriteLine();
    }

    options.View = new ProjectView(columns);
    options.PresentationFormat = PresentationFormat.ResourceUsage;

    project.Save(OutDir + "WorkWithViewColumn_out.pdf", options);
}

private class MyTextStyleCallback : ITextStyleModificationCallback
{
    /// <summary>
    /// टास्क पंक्ति के लिए टेबल सेल को रेंडर करने से पहले बुलाई जाने वाली विधि निम्नलिखित दृश्यों में:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'।
    /// </summary>
    /// <param name=\"args\">यह <see cref=\"T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs\" /> ऑब्जेक्ट।</param>
    public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
    {
        if (args.Task.Get(Tsk.Uid) % 2 == 0)
        {
            args.CellTextStyle.BackgroundColor = 
                args.Column.StringAlignment == HorizontalStringAlignment.Center 
                ? Color.Cyan : Color.Red;
            args.CellTextStyle.BackgroundPattern = BackgroundPattern.SolidFill;
        }
        else
        {
            args.CellTextStyle.Color = Color.DarkGreen;
        }
    }
}
```

### संबंधित देखें

* class [TaskTextStyleEventArgs](../../tasktextstyleeventargs/)
* interface [ITextStyleModificationCallback](../)
* namespace [Aspose.Tasks.Visualization](../../itextstylemodificationcallback/)
* assembly [Aspose.Tasks](../../../)


