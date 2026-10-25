---
title: "Enum FileFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.FileFormat enum. Menentukan format file proyek"
type: docs
weight: 590
url: /id/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

Menentukan format file proyek.

```csharp
public enum FileFormat
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `0` | Tidak dapat didefinisikan. |
| P6XML | `1` | Mewakili format XML Primavera P6. |
| XML | `2` | Format XML Microsoft Project. |
| MPP8 | `3` | Format Microsoft Project 2000. |
| MPP9 | `4` | Format Microsoft Project 2003. |
| MPP12 | `5` | Format Microsoft Project 2007. |
| MPP14 | `6` | Format Microsoft Project 2010. |
| MPT9 | `7` | Format templat Microsoft Project 2003. |
| MPT12 | `8` | Format templat Microsoft Project 2007. |
| MPT14 | `9` | Format templat Microsoft Project 2010 (2013). |
| MPX | `10` | Format berkas Mpx |
| XER | `11` | Mewakili format Primavera XER |
| HTML | `12` | Mewakili format HTML |
| ProjectServer | `13` | Proyek dibaca dari Project Server atau Project Online |

## Contoh

Menampilkan cara membaca format berkas proyek check.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


