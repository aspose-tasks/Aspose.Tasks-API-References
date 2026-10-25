---
title: "MPPSaveOptions.RemoveInvalidAssignments"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MPPSaveOptions प्रॉपर्टी। यह मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि MPP में सहेजते समय अमान्य रिसोर्स असाइनमेंट्स हटाए जाएँ या नहीं। MS Project प्रत्येक टास्क के लिए एक खाली रिसोर्स असाइनमेंट बनाता है। इस फ़्लैग को true सेट करने पर सहेजते समय इन्हें हटाया जाएगा।"
type: docs
weight: 40
url: /hi/net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

MPP में सहेजते समय अमान्य संसाधन असाइनमेंट को हटाने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। MS Project प्रत्येक कार्य के लिए एक खाली संसाधन असाइनमेंट बनाता है। सहेजते समय उन्हें हटाने के लिए इस फ़्लैग को true सेट करें।

```csharp
public bool RemoveInvalidAssignments { get; set; }
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


