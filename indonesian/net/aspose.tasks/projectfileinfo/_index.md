---
title: "Kelas ProjectFileInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ProjectFileInfo. Instance kelas ini berisi informasi tentang format file proyek dan versi Microsoft Project tempat file tersebut dibuat."
type: docs
weight: 1460
url: /id/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

Instansi kelas ini berisi informasi tentang format file proyek dan versi Microsoft Project tempat file tersebut dibuat.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Mendapatkan nilai yang menunjukkan apakah Aspose.Tasks dapat memproses file proyek. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | Mendapatkan nilai yang menunjukkan apakah proyek dilindungi kata sandi. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | Mendapatkan info aplikasi file proyek. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | Mendapatkan format file proyek. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | Mengembalikan nilai kode hash untuk instance dari kelas `ProjectFileInfo`. |

## Catatan

Gunakan properti CanRead untuk menentukan bahwa perpustakaan dapat memproses file proyek.

## Contoh

Menampilkan cara membaca informasi file proyek.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


