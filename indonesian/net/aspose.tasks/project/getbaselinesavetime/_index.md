---
title: "Project.GetBaselineSaveTime"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Mengembalikan waktu penyimpanan baseline"
type: docs
weight: 1090
url: /id/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

Mengembalikan waktu penyimpanan baseline.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| baselineNumber | BaselineType | Nomor baseline [`BaselineType`](../../baselinetype/). |

### Nilai Kembali

Tanggal dan waktu penyimpanan terakhir baseline.

## Catatan

Mengembalikan DateTime.MinValue jika baseline tidak disimpan.

## Contoh

Menampilkan cara membaca/menulis waktu penyimpanan baseline proyek.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// atur waktu penyimpanan baseline
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### Lihat Juga

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


