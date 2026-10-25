---
title: "VbaModule.Name"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModule प्रॉपर्टी। VBA मॉड्यूल का नाम प्राप्त करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

VBA मॉड्यूल का नाम प्राप्त करता है

```csharp
public string Name { get; set; }
```

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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


