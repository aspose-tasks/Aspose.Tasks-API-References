---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraBaseReader मेथड। प्रोजेक्ट्स के अद्वितीय पहचानकर्ताओं की सूची लौटाता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

परियोजनाओं के अद्वितीय पहचानकर्ताओं की सूची लौटाएँ।

```csharp
public List<int> GetProjectUids()
```

### रिटर्न वैल्यू

परियोजनाओं के अद्वितीय पहचानकर्ताओं की सूची।

## उदाहरण

Primavera XML फ़ाइल से प्रोजेक्ट आयात करने का तरीका दिखाता है।

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### संबंधित देखें

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


