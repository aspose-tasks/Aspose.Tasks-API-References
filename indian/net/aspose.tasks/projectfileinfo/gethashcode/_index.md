---
title: "ProjectFileInfo.GetHashCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectFileInfo मेथड। ProjectFileInfo क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

[`ProjectFileInfo`](../) क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है।

```csharp
public override int GetHashCode()
```

### रिटर्न वैल्यू

इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।

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


