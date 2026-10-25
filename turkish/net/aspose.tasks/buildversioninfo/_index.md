---
title: "Sınıf BuildVersionInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.BuildVersionInfo sınıfı. Derleme sürümü ve ürün bilgilerini içerir"
type: docs
weight: 160
url: /tr/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

Derleme sürümünü ve ürün bilgilerini içerir.

```csharp
public static class BuildVersionInfo
```

## Alanlar

| Ad | Açıklama |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | Derlemenin bilgi sürüm numarası. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | Derleme sürümü. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | Dosya sürümü. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | Ürün adı. |

## Örnekler

Aspose.Tasks'ın derleme sürüm bilgilerini nasıl okuyacağınızı gösterir.

```csharp
// geçerli Aspose.Tasks sürümü hakkında ortak bilgileri oku
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


