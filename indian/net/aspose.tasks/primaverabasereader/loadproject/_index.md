---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraBaseReader मेथड। निर्दिष्ट अद्वितीय पहचानकर्ता वाले प्रोजेक्ट को लोड करता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

निर्दिष्ट अद्वितीय पहचानकर्ता वाले परियोजना को लोड करता है।

```csharp
public virtual Project LoadProject(int projectUid)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectUid | Int32 | लोड करने वाले प्रोजेक्ट का अद्वितीय पहचानकर्ता। |

### रिटर्न वैल्यू

निर्दिष्ट मल्टी प्रोजेक्ट फ़ाइल से निर्दिष्ट अद्वितीय पहचानकर्ता वाला प्रोजेक्ट। यदि प्रोजेक्ट मौजूद नहीं है तो Null।

## उदाहरण

जब प्रोजेक्ट UID ज्ञात हो, तब Primavera XML फ़ाइल से प्रोजेक्ट लोड करने का तरीका दिखाता है।

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

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

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


