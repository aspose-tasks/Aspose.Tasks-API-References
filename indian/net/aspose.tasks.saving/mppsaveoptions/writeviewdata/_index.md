---
title: "MPPSaveOptions.WriteViewData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MPPSaveOptions प्रॉपर्टी। यह मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय व्यू डेटा लिखा जाए या नहीं। व्यू डेटा में Project.Views, Filters और Tables संग्रह शामिल हैं।"
type: docs
weight: 80
url: /hi/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय व्यू डेटा लिखने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। व्यू डेटा में Project.Views, Filters और Tables संग्रह शामिल हैं।

```csharp
public bool WriteViewData { get; set; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को स्ट्रीम में MPP फ़ाइल के रूप में कैसे सहेजा जाए।

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // सेव विकल्प बनाएं
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // MPP में सहेजते समय अमान्य संसाधन असाइनमेंट को हटाने का संकेत देने वाला मान सेट करता है
        RemoveInvalidAssignments = true
    };

    // विकल्पों के साथ MPP सहेजें
    project.Save(stream, options);
}
```

### संबंधित देखें

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


