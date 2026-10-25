---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MPPSaveOptions प्रॉपर्टी। यह पासवर्ड प्राप्त करता है या सेट करता है जिसका उपयोग परिणामी MPP फ़ाइल को सुरक्षित करने के लिए किया जाता है। वर्तमान में MS Project 2010 और नए फ़ॉर्मेट्स के लिए समर्थित है। null मान दर्शाता है कि प्रोजेक्ट फ़ाइल सुरक्षित नहीं है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

परिणामी MPP फ़ाइल की सुरक्षा के लिए उपयोग किया जाने वाला पासवर्ड प्राप्त करता है या सेट करता है। वर्तमान में MS Project 2010 और नए फ़ॉर्मेट्स के लिए समर्थित है। शून्य मान दर्शाता है कि प्रोजेक्ट फ़ाइल संरक्षित नहीं है।

```csharp
public string ProtectionPassword { get; set; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को पासवर्ड-प्रोटेक्टेड MPP फ़ाइल में कैसे सहेजें।

```csharp
try
{

    var project = new Project(DataDir + "Project1.mpp");

    SimpleSaveOptions options = new MPPSaveOptions
    {
        ProtectionPassword = "password!234"
    };

    project.Save(OutDir + "PasswordProtected.mpp", options);
}
catch (NotSupportedException ex)
{
    Console.WriteLine(ex.Message + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
}
```

### संबंधित देखें

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


