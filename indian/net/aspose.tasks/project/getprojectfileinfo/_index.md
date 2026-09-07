---
title: "Project.GetProjectFileInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। फ़ाइल से प्रोजेक्ट फ़ाइल जानकारी पढ़ता है"
type: docs
weight: 1280
url: /hi/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

फ़ाइल से परियोजना फ़ाइल जानकारी पढ़ता है।

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ाइलनाम | स्ट्रिंग | प्रोजेक्ट फ़ाइलनाम। |

### रिटर्न वैल्यू

प्रोजेक्ट फ़ाइल जानकारी [`ProjectFileInfo`](../../projectfileinfo/).

## उदाहरण

XML फ़ाइल से पढ़ी गई प्रोजेक्ट फ़ाइल जानकारी को पढ़ने का तरीका दिखाता है।

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### संबंधित देखें

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

स्ट्रीम से परियोजना फ़ाइल जानकारी प्राप्त करता है।

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | डेटा स्ट्रीम। |

### रिटर्न वैल्यू

प्रोजेक्ट फ़ाइल जानकारी [`ProjectFileInfo`](../../projectfileinfo/).

## उदाहरण

स्ट्रीम से पढ़ी गई XML फ़ाइल की प्रोजेक्ट फ़ाइल जानकारी को पढ़ने का तरीका दिखाता है।

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### संबंधित देखें

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


