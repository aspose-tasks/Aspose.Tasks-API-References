---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectFileInfo प्रॉपर्टी। प्रोजेक्ट फ़ाइल फ़ॉर्मेट प्राप्त करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

प्रोजेक्ट फ़ाइल फ़ॉर्मेट प्राप्त करता है।

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


