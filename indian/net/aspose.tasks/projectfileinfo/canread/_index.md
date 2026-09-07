---
title: "ProjectFileInfo.CanRead"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectFileInfo प्रॉपर्टी। एक मान प्राप्त करता है जो दर्शाता है कि क्या defines Aspose.Tasks प्रोजेक्ट फ़ाइल को प्रोसेस कर सकते हैं"
type: docs
weight: 10
url: /hi/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Aspose.Tasks प्रोजेक्ट फ़ाइल को प्रोसेस कर सकता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

```csharp
public bool CanRead { get; }
```

## उदाहरण

प्रोजेक्ट फ़ाइल की जानकारी पढ़ने का तरीका दर्शाता है।

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### संबंधित देखें

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


