---
title: "क्लास ProjectFileInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ProjectFileInfo क्लास। क्लास का उदाहरण प्रोजेक्ट फ़ाइल फ़ॉर्मेट और उस माइक्रोसॉफ्ट प्रोजेक्ट संस्करण की जानकारी रखता है जिसमें फ़ाइल बनाई गई थी।"
type: docs
weight: 1460
url: /hi/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

क्लास इंस्टेंस में प्रोजेक्ट फ़ाइल फ़ॉर्मेट और Microsoft Project के संस्करण के बारे में जानकारी होती है जहाँ फ़ाइल बनाई गई थी।

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Aspose.Tasks प्रोजेक्ट फ़ाइल को प्रोसेस कर सकता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | प्रोजेक्ट पासवर्ड से सुरक्षित है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | प्रोजेक्ट फ़ाइल एप्लिकेशन जानकारी प्राप्त करता है। |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | प्रोजेक्ट फ़ाइल फ़ॉर्मेट प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | `ProjectFileInfo` क्लास के उदाहरण के लिए हैश कोड मान लौटाता है। |

## टिप्पणियाँ

CanRead प्रॉपर्टी का उपयोग करके निर्धारित करें कि लाइब्रेरी प्रोजेक्ट फ़ाइल को प्रोसेस कर सकती है।

## उदाहरण

प्रोजेक्ट फ़ाइल की जानकारी पढ़ने का तरीका दर्शाता है।

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


