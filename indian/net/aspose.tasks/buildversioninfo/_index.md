---
title: "क्लास BuildVersionInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.BuildVersionInfo क्लास। इसमें बिल्ड संस्करण और उत्पाद जानकारी शामिल है।"
type: docs
weight: 160
url: /hi/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

बिल्ड संस्करण और उत्पाद जानकारी शामिल है।

```csharp
public static class BuildVersionInfo
```

## फ़ील्ड्स

| नाम | विवरण |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | असेंबली का सूचना संस्करण संख्या। |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | असेंबली संस्करण। |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | फ़ाइल संस्करण। |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | उत्पाद नाम। |

## उदाहरण

विवरण देता है कि Aspose.Tasks का बिल्ड संस्करण जानकारी कैसे पढ़ें।

```csharp
// वर्तमान Aspose.Tasks संस्करण के बारे में सामान्य जानकारी पढ़ें
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


