---
title: "VbaProject.References"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaProject प्रॉपर्टी। VbaReferenceCollection का संग्रह प्राप्त करता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

[`VbaReferenceCollection`](../../vbareferencecollection/) का संग्रह प्राप्त करता है

```csharp
public VbaReferenceCollection References { get; }
```

## उदाहरण

दिखाता है कि VBA प्रोजेक्ट रेफ़रेंस जानकारी कैसे पढ़ें।

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

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


