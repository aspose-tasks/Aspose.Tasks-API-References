---
title: "क्लास TaskTextStyleEventArgs"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.TaskTextStyleEventArgs क्लास। यह क्लास टेबल सेल की सामग्री के रेंडरिंग से संबंधित डेटा सेट का प्रतिनिधित्व करती है"
type: docs
weight: 3390
url: /hi/net/aspose.tasks.visualization/tasktextstyleeventargs/
---
## TaskTextStyleEventArgs class

यह वर्ग तालिका सेल की सामग्री के रेंडरिंग से संबंधित डेटा सेट को दर्शाता है।

```csharp
public class TaskTextStyleEventArgs
```

## गुण

| नाम | विवरण |
| --- | --- |
| [CellTextStyle](../../aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/) { get; set; } | सेल की सामग्री को ड्रॉ करने के लिए उपयोग किए जाने वाले TextStyle को प्राप्त करता है या सेट करता है। इस ऑब्जेक्ट का उपयोग टेबल सेल की उपस्थिति को अनुकूलित करने के लिए किया जा सकता है। |
| [Column](../../aspose.tasks.visualization/tasktextstyleeventargs/column/) { get; } | उस [`ViewColumn`](../viewcolumn/) को प्राप्त करता है जिससे वर्तमान में रेंडर किया गया सेल संबंधित है। |
| [Task](../../aspose.tasks.visualization/tasktextstyleeventargs/task/) { get; } | उस [`Task`](./task/) को प्राप्त करता है जो वर्तमान में रेंडर की गई पंक्ति से मेल खाता है। |

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


