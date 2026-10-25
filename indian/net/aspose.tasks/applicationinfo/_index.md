---
title: "Enum ApplicationInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ApplicationInfo enum। फ़ाइल के निर्मित होने वाले प्रोजेक्ट संस्करण को निर्दिष्ट करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

फ़ाइल के निर्मित होने वाले परियोजना संस्करण को निर्दिष्ट करता है।

```csharp
public enum ApplicationInfo
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `0` | परिभाषित नहीं किया जा सकता। |
| MSP2000 | `1` | फ़ाइल Microsoft Project 2000/2002 में बनाई गई थी। |
| MSP2003 | `2` | फ़ाइल Microsoft Project 2003 में बनाई गई थी। |
| MSP2007 | `3` | फ़ाइल Microsoft Project 2007 में बनाई गई थी। |
| MSP2010 | `4` | फ़ाइल Microsoft Project 2010 में बनाई गई थी। |
| MSP2013 | `5` | फ़ाइल Microsoft Project 2013 में बनाई गई थी। |
| MSP2016 | `6` | फ़ाइल Microsoft Project 2016 में बनाई गई थी। |

## उदाहरण

प्रोजेक्ट एप्लिकेशन जानकारी की जाँच करने का तरीका दिखाता है।

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


