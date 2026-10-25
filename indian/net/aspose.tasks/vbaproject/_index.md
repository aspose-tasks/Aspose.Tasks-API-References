---
title: "क्लास VbaProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.VbaProject क्लास। VbaProject का प्रतिनिधित्व करता है।"
type: docs
weight: 2860
url: /hi/net/aspose.tasks/vbaproject/
---
## VbaProject class

`VbaProject` का प्रतिनिधित्व करता है।

```csharp
public class VbaProject
```

## गुण

| नाम | विवरण |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | शर्तीय संकलन तर्क प्राप्त करता है |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | परियोजना विवरण प्राप्त करता है। |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | परियोजना हेल्प कॉन्टेक्स्ट आईडी प्राप्त करता है। |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | हेल्प फ़ाइल का नाम प्राप्त करता है। |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | [`VbaModuleCollection`](../vbamodulecollection/) का संग्रह प्राप्त करता है। |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | परियोजना नाम प्राप्त करता है। |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | [`VbaReferenceCollection`](../vbareferencecollection/) का संग्रह प्राप्त करता है। |

## उदाहरण

विवरण देता है कि VBA प्रोजेक्ट गुणों को कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


