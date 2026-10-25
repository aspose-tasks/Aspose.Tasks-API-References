---
title: "Enum ApplicationInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.ApplicationInfo. Menentukan versi proyek tempat file dibuat."
type: docs
weight: 10
url: /id/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

Menentukan versi proyek tempat file dibuat.

```csharp
public enum ApplicationInfo
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `0` | Tidak dapat didefinisikan. |
| MSP2000 | `1` | File dibuat di Microsoft Project 2000/2002. |
| MSP2003 | `2` | File dibuat di Microsoft Project 2003. |
| MSP2007 | `3` | File dibuat di Microsoft Project 2007. |
| MSP2010 | `4` | File dibuat di Microsoft Project 2010. |
| MSP2013 | `5` | File dibuat di Microsoft Project 2013. |
| MSP2016 | `6` | File dibuat di Microsoft Project 2016. |

## Contoh

Menampilkan cara memeriksa info aplikasi proyek.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


