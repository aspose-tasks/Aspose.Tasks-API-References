---
title: "Kelas BuildVersionInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.BuildVersionInfo. Berisi informasi versi build dan produk."
type: docs
weight: 160
url: /id/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

Berisi versi build dan informasi produk.

```csharp
public static class BuildVersionInfo
```

## Bidang

| Nama | Deskripsi |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | Nomor versi informasional dari assembly. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | Versi assembly. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | Versi file. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | Nama produk. |

## Contoh

Menampilkan cara membaca informasi versi build dari Aspose.Tasks.

```csharp
// baca info umum tentang versi Aspose.Tasks saat ini
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


