---
title: "क्लास **VbaReference**"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "**Aspose.Tasks.VbaReference** क्लास। VbaProject का एक संदर्भ दर्शाता है।"
type: docs
weight: 2870
url: /hi/net/aspose.tasks/vbareference/
---
## VbaReference class

[`VbaProject`](../vbaproject/) का एक संदर्भ दर्शाता है।

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [VbaReference](vbareference/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | लाइब्रेरी की पहचानकर्ता प्राप्त करता है। |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | VBA संदर्भ का नाम प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट `VbaReference` ऑब्जेक्ट के बराबर है या नहीं। |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | यह मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट `VbaReference` ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | इस `VbaReference` के लिए हैश कोड मान लौटाता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


