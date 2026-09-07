---
title: "क्लास LoadOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.LoadOptions क्लास। फ़ाइल या स्ट्रीम से प्रोजेक्ट लोड करते समय अतिरिक्त लोड पैरामीटर निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 990
url: /hi/net/aspose.tasks/loadoptions/
---
## LoadOptions class

फ़ाइल या स्ट्रीम से प्रोजेक्ट लोड करते समय अतिरिक्त लोड पैरामीटर निर्दिष्ट करने की अनुमति देता है।

```csharp
public class LoadOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [LoadOptions](loadoptions/)() | `LoadOptions` क्लास का एक नया इंस्टेंस प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | प्रोजेक्ट लोडिंग ऑपरेशन को रद्द करने के लिए उपयोग किए जा सकने वाले टोकन को प्राप्त करता है या सेट करता है। |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | HTML, MPX, XER और Primavera XML फ़ॉर्मेट्स से प्रोजेक्ट पढ़ने के लिए उपयोग की जाने वाली एन्कोडिंग को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट एन्कोडिंग UTF8 है। |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | XML पार्स त्रुटियों को संभालने के लिए कॉलबैक मेथड को प्राप्त करता है या सेट करता है। |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | प्रोटेक्शन पासवर्ड को प्राप्त करता है या सेट करता है। |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | [`PrimaveraReadOptions`](../primaverareadoptions/) क्लास का निर्दिष्ट इंस्टेंस प्राप्त करता है या सेट करता है, जिसका उपयोग Primavera फ़ॉर्मेट्स (Primavera P6 XER या Primavera P6 Xml) को लोड करने के व्यवहार को अनुकूलित करने के लिए किया जा सकता है। |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | प्रोजेक्ट लोडिंग ऑपरेशन्स के दौरान बुलाए जाने वाले कॉलबैक को प्राप्त करता है या सेट करता है। वर्तमान में MPP और XER फ़ॉर्मेट्स के लिए समर्थित है। |

## उदाहरण

<see cref=\"Aspose.Tasks.LoadOptions\"/> इंस्टेंस का उपयोग करके पासवर्ड-प्रोटेक्टेड प्रोजेक्ट को लोड करने का तरीका दिखाता है।

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


