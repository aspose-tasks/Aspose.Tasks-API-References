---
title: "क्लास VbaModule"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.VbaModule क्लास। एक VBA मॉड्यूल का प्रतिनिधित्व करता है"
type: docs
weight: 2810
url: /hi/net/aspose.tasks/vbamodule/
---
## VbaModule class

एक VBA मॉड्यूल का प्रतिनिधित्व करता है।

```csharp
public sealed class VbaModule
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | मॉड्यूल के गुणों का संग्रह प्राप्त करता है। |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | VBA मॉड्यूल का नाम प्राप्त करता है |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | VBA मॉड्यूल का स्रोत कोड प्राप्त करता है या सेट करता है |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | मॉड्यूल का प्रकार प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | `VbaModule` का एक उदाहरण बनाता है जिसमें VbaModuleType.ClassModule प्रकार हो। |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | `VbaModule` का एक उदाहरण बनाता है जिसमें VbaModuleType.ProceduralModule प्रकार हो। |

## उदाहरण

दिखाता है कि VBA प्रोजेक्ट के मॉड्यूल कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


