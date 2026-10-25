---
title: "VbaReference.LibIdentifier"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaReference property. लाइब्रेरी का पहचानकर्ता प्राप्त करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

लाइब्रेरी की पहचानकर्ता प्राप्त करता है।

```csharp
public string LibIdentifier { get; }
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


