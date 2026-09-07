---
title: "क्लास PrimaveraDbReader"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.PrimaveraDbReader क्लास। Primavera DB से प्रोजेक्ट जानकारी पढ़ने के लिए एक रीडर का प्रतिनिधित्व करता है।"
type: docs
weight: 1350
url: /hi/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Primavera DB से प्रोजेक्ट जानकारी पढ़ने के लिए एक रीडर का प्रतिनिधित्व करता है।

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | [`PrimaveraXerReader`](../primaveraxerreader/) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | प्रोजेक्ट की शॉर्ट इन्फो ऑब्जेक्ट्स की सूची लौटाता है। |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | परियोजनाओं के अद्वितीय पहचानकर्ताओं की सूची लौटाएँ। |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | निर्दिष्ट अद्वितीय पहचानकर्ता वाले परियोजना को लोड करता है। |

## उदाहरण

Primavera डेटाबेस से परियोजनाओं की संक्षिप्त जानकारी कैसे प्राप्त करें, यह दर्शाता है।

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### संबंधित देखें

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


