---
title: "Enum DataCategory"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Saving.DataCategory. Kategori data yang digunakan saat menyimpan ke CSV"
type: docs
weight: 2000
url: /id/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

Kategori data yang digunakan saat menyimpan ke CSV.

```csharp
public enum DataCategory
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Tasks | `0` | Informasi tugas. |
| Resources | `1` | Informasi sumber daya. |
| Assignments | `2` | Informasi penugasan. |

## Contoh

Menampilkan cara menggunakan &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; untuk menyimpan proyek sebagai file CSV.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

### Lihat Juga

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


