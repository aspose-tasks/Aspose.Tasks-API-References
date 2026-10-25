---
title: "Enum GanttBarFillPattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.GanttBarFillPattern enum. आकार का भराव पैटर्न"
type: docs
weight: 3040
url: /hi/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

एक आकार का भराव पैटर्न।

```csharp
public enum GanttBarFillPattern
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Hollow | `0` | खाली पैटर्न। |
| SolidFill | `1` | ठोस भराव पैटर्न। |
| LightFill | `2` | हल्का भराव पैटर्न। |
| MediumFill | `3` | मध्यम भराव पैटर्न। |
| DarkFill | `4` | गहरा भराव पैटर्न। |
| DiagonalLeft | `5` | डायगोनल बायाँ पैटर्न (ऊपर बाएँ से नीचे दाएँ तक)। |
| DiagonalRight | `6` | डायगोनल दायाँ पैटर्न (ऊपर दाएँ से नीचे बाएँ तक)। |
| DiagonalCross | `7` | विकर्ण क्रॉस पैटर्न। |
| LineVertical | `8` | वर्टिकल लाइन पैटर्न। |
| LineHorizontal | `9` | हॉरिज़ॉन्टल लाइन पैटर्न। |
| LineCross | `10` | क्रॉस लाइन पैटर्न। |
| SolidFillWithDashedBorder | `11` | डैश्ड बॉर्डर के साथ सॉलिड पैटर्न। |

## उदाहरण

दिखाता है कि Gantt चार्ट प्रोजेक्ट व्यू की कस्टम बार शैलियों को कैसे सेट किया जाए।

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // कस्टम बार शैली को प्रोजेक्ट व्यू के कस्टम बार संग्रह में जोड़ें।
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


