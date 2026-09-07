---
title: "MPPSaveOptions.ClearVba"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MPPSaveOptions प्रॉपर्टी। यह मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय मौजूदा VBA मैक्रो डेटा हटाया जाए या नहीं।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

प्रोजेक्ट को MPP फ़ॉर्मेट में सहेजते समय मौजूदा VBA मैक्रो डेटा को हटाने का संकेत देने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool ClearVba { get; set; }
```

## उदाहरण

MPP फ़ाइल से VBA मैक्रो को हटाने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### संबंधित देखें

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


