---
title: "Project.SetBaselineSaveTime"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Mengatur waktu penyimpanan baseline"
type: docs
weight: 1260
url: /id/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

Mengatur waktu penyimpanan baseline.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| baselineNumber | BaselineType | Nomor baseline [`BaselineType`](../../baselinetype/). |
| value | DateTime | Tanggal dan waktu penyimpanan terakhir baseline. |

## Catatan

Set nilai ke DateTime.MinValue jika baseline tidak disimpan.

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


