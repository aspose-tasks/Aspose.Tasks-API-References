---
title: "क्लास PrimaveraXerReader"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.PrimaveraXerReader क्लास। Primavera XER फ़ाइल से प्रोजेक्ट UID पढ़ने के लिए रीडर का प्रतिनिधित्व करता है।"
type: docs
weight: 1390
url: /hi/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Primavera XER फ़ाइल से प्रोजेक्ट UID पढ़ने के लिए एक रीडर का प्रतिनिधित्व करता है।

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | `PrimaveraXerReader` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | `PrimaveraXerReader` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | प्रोजेक्ट की शॉर्ट इन्फो ऑब्जेक्ट्स की सूची लौटाता है। |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | परियोजनाओं के अद्वितीय पहचानकर्ताओं की सूची लौटाएँ। |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | निर्दिष्ट अद्वितीय पहचानकर्ता वाले परियोजना को लोड करता है। |

## उदाहरण

दिखाता है कि Primavera XER फ़ाइल से छोटे प्रोजेक्ट्स की जानकारी कैसे जांचें।

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### संबंधित देखें

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


