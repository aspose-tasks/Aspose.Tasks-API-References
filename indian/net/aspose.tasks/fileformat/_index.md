---
title: "Enum FileFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.FileFormat enum. प्रोजेक्ट्स फ़ाइल फ़ॉर्मेट निर्दिष्ट करता है"
type: docs
weight: 590
url: /hi/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

परियोजना के फ़ाइल प्रारूप को निर्दिष्ट करता है।

```csharp
public enum FileFormat
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `0` | परिभाषित नहीं किया जा सकता। |
| P6XML | `1` | Primavera P6 XML फ़ॉर्मेट का प्रतिनिधित्व करता है। |
| XML | `2` | Microsoft Project XML फ़ॉर्मेट। |
| MPP8 | `3` | Microsoft Project 2000 फ़ॉर्मेट। |
| MPP9 | `4` | Microsoft Project 2003 फ़ॉर्मेट। |
| MPP12 | `5` | Microsoft Project 2007 फ़ॉर्मेट। |
| MPP14 | `6` | Microsoft Project 2010 फ़ॉर्मेट। |
| MPT9 | `7` | Microsoft Project 2003 टेम्पलेट फ़ॉर्मेट। |
| MPT12 | `8` | Microsoft Project 2007 टेम्पलेट फ़ॉर्मेट। |
| MPT14 | `9` | Microsoft Project 2010 (2013) टेम्प्लेट फ़ॉर्मेट। |
| MPX | `10` | Mpx फ़ाइल फ़ॉर्मेट |
| XER | `11` | Primavera XER फ़ॉर्मेट का प्रतिनिधित्व करता है |
| HTML | `12` | HTML फ़ॉर्मेट का प्रतिनिधित्व करता है |
| ProjectServer | `13` | प्रोजेक्ट को Project Server या Project Online से पढ़ा गया था |

## उदाहरण

दिखाता है कि प्रोजेक्ट फ़ाइल फ़ॉर्मेट को कैसे पढ़ें और जांचें।

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


