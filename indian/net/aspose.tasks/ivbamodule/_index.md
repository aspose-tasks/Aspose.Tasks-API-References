---
title: "इंटरफ़ेस IVbaModule"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.IVbaModule इंटरफ़ेस। VBA कोड वाला मॉड्यूल दर्शाता है"
type: docs
weight: 880
url: /hi/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

VBA कोड वाला मॉड्यूल दर्शाता है।

```csharp
public interface IVbaModule
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) का संग्रह प्राप्त करता है। |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | VBA मॉड्यूल का नाम प्राप्त करता है |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | VBA मॉड्यूल का स्रोत कोड प्राप्त करता है। |

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


