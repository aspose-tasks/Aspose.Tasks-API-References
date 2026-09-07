---
title: "VbaReference.Name"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaReference प्रॉपर्टी। इस VBA रेफ़रेंस का नाम प्राप्त करता है या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

VBA संदर्भ का नाम प्राप्त करता है या सेट करता है।

```csharp
public string Name { get; set; }
```

## उदाहरण

VBA संदर्भों को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### संबंधित देखें

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


