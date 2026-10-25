---
title: "Prj.WorkFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Format yang digunakan untuk menampilkan durasi tugas"
type: docs
weight: 790
url: /id/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

Format yang digunakan untuk menampilkan durasi tugas.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## Contoh

Menunjukkan cara mendapatkan durasi dengan format kerja default.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// buat nilai work dengan format kerja default proyek
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


