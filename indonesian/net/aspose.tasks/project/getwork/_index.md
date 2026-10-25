---
title: "Project.GetWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Mendapatkan objek Duration dengan nilai Double yang ditentukan dan format kerja default"
type: docs
weight: 1130
url: /id/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

Mendapatkan objek [`Duration`](../../duration/) dengan nilai Double yang ditentukan dan format kerja default.

```csharp
public Duration GetWork(double val)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| val | Double | nilai double yang ditentukan. |

### Nilai Kembali

Objek Duration.

## Catatan

Metode ini harus digunakan dengan hati-hati karena mengembalikan durasi yang berbeda tergantung pada pengaturan Project.WorkFormat. Misalnya, GetWork(1.0) akan mengembalikan 1 jam ketika Project.WorkFormat adalah TimeUnitType.Hour atau 1 hari jika Project.WorkFormat adalah TimeUnitType.Day.

## Contoh

Menampilkan cara mendapatkan work dengan format kerja default.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// buat nilai work dengan format kerja default proyek
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Lihat Juga

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


