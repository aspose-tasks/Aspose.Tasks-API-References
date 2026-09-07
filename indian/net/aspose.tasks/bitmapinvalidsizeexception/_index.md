---
title: "Class BitmapInvalidSizeException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.BitmapInvalidSizeException class. जब बिटमैप इंस्टेंस बनाने के लिए पर्याप्त मेमोरी नहीं होती है, तब उत्पन्न होने वाले अपवाद का प्रतिनिधित्व करता है।"
type: docs
weight: 140
url: /hi/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

एक अपवाद का प्रतिनिधित्व करता है जो तब उत्पन्न होता है जब बिटमैप इंस्टेंस बनाने के लिए पर्याप्त मेमोरी नहीं होती।

```csharp
public class BitmapInvalidSizeException : Exception
```

## उदाहरण

दिखाता है कि कैसे प्रोजेक्ट को छवि के रूप में सहेजें और अवैध आकार अपवाद को पकड़ें।

```csharp
try
{
    var project = new Project(DataDir + "Blank2010.mpp");

    GanttChartView view = (GanttChartView) project.Views.ToList()[0];
    var options = new ImageSaveOptions(SaveFileFormat.Png)
    {
        Timescale = Timescale.DefinedInView
    };

    view.MiddleTimescaleTier.Unit = TimescaleUnit.Minutes;
    view.MiddleTimescaleTier.Count = 1;

    project.Save(OutDir + "SaveToStreamAndCatchException_out.mpp", options);
}
catch (BitmapInvalidSizeException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


