---
title: "क्लास ApsLayoutBuilderOutOfMemoryException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException क्लास। वह अपवाद दर्शाता है जो तब होता है जब इमेज लेआउट निर्माण जारी रखने के लिए पर्याप्त मेमोरी नहीं होती।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

एक अपवाद को दर्शाता है जो तब होता है जब इमेज लेआउट निर्माण जारी रखने के लिए पर्याप्त मेमोरी नहीं होती।

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को इमेज के रूप में कैसे सहेजें और अपवादों को कैसे पकड़ें।

```csharp
try
{
    var project = new Project(DataDir + "Blank2010.mpp");

    var ganttChart = (GanttChartView)project.Views.ToList()[0];

    ganttChart.MiddleTimescaleTier.Unit = TimescaleUnit.Hours;
    ganttChart.BottomTimescaleTier.Unit = TimescaleUnit.Minutes;
    ganttChart.BottomTimescaleTier.Count = 1;

    var options = new ImageSaveOptions(SaveFileFormat.Png);
    options.Timescale = Timescale.DefinedInView;

    project.Save(OutDir + "SaveToStreamWithOptionsAndCatchException_out.mpp", options);
}
catch (ApsLayoutBuilderOutOfMemoryException ex)
{
    Console.WriteLine(ex.Message);
}
catch (BitmapInvalidSizeException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


