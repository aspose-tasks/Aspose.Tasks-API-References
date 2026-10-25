---
title: "इंटरफ़ेस ITextStyleModificationCallback"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.ITextStyleModificationCallback इंटरफ़ेस। यह एक कॉलबैक का प्रतिनिधित्व करता है जो टेबल सेल पर TextStyle लागू करने से पहले बुलाया जाता है"
type: docs
weight: 3160
url: /hi/net/aspose.tasks.visualization/itextstylemodificationcallback/
---
## ITextStyleModificationCallback interface

एक कॉलबैक का प्रतिनिधित्व करता है जो टेबल सेल पर TextStyle लागू होने से पहले बुलाया जाता है।

```csharp
public interface ITextStyleModificationCallback
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [BeforeTaskTextStyleApplied](../../aspose.tasks.visualization/itextstylemodificationcallback/beforetasktextstyleapplied/)(TaskTextStyleEventArgs) | निम्नलिखित दृश्यों में टास्क पंक्ति के लिए टेबल सेल को रेंडर करने से पहले बुलाई जाने वाली विधि: 'Gantt Chart', 'Task Sheet', 'Task Usage'। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


