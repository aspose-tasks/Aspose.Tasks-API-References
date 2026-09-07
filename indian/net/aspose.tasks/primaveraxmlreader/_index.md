---
title: "क्लास PrimaveraXmlReader"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.PrimaveraXmlReader क्लास। एक रीडर का प्रतिनिधित्व करता है जो Primavera Xml फ़ाइल से प्रोजेक्ट UID प्राप्त करने की अनुमति देता है।"
type: docs
weight: 1400
url: /hi/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

एक रीडर का प्रतिनिधित्व करता है जो Primavera XML फ़ाइल से प्रोजेक्ट UID पुनः प्राप्त करने की अनुमति देता है।

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | `PrimaveraXmlReader` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | `PrimaveraXmlReader` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | प्रोजेक्ट की शॉर्ट इन्फो ऑब्जेक्ट्स की सूची लौटाता है। |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | परियोजनाओं के अद्वितीय पहचानकर्ताओं की सूची लौटाएँ। |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | निर्दिष्ट अद्वितीय पहचानकर्ता वाले परियोजना को लोड करता है। |

## उदाहरण

एक Primavera XML फ़ाइल से छोटे प्रोजेक्ट्स की जानकारी की जांच कैसे करें, यह दिखाता है।

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### संबंधित देखें

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


