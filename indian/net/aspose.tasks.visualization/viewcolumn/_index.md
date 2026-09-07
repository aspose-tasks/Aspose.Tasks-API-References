---
title: "क्लास ViewColumn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.ViewColumn क्लास। यह प्रोजेक्ट दृश्य में एक कॉलम का प्रतिनिधित्व करता है"
type: docs
weight: 3470
url: /hi/net/aspose.tasks.visualization/viewcolumn/
---
## ViewColumn class

प्रोजेक्ट व्यू में एक कॉलम का प्रतिनिधित्व करता है।

```csharp
public abstract class ViewColumn
```

## गुण

| नाम | विवरण |
| --- | --- |
| abstract [Field](../../aspose.tasks.visualization/viewcolumn/field/) { get; set; } | कॉलम फ़ील्ड को प्राप्त करता है या सेट करता है। [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | कॉलम का नाम प्राप्त करता है। |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | पाठ की संरेखण प्राप्त करता है या सेट करता है (यह [`HorizontalStringAlignment`](../horizontalstringalignment/) enumeration के मानों में से एक हो सकता है)। |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | कॉलम की कोशिकाओं की उपस्थिति को अनुकूलित करने के लिए उपयोग की जा सकने वाली कॉलबैक प्राप्त करता है या सेट करता है। |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | कॉलम की चौड़ाई प्राप्त करता है। |

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


