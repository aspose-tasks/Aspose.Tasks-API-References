---
title: "Enum CsvTextDelimiter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Saving.CsvTextDelimiter. Pembatas teks untuk format CSV"
type: docs
weight: 1990
url: /id/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

Pembatas teks untuk format CSV.

```csharp
public enum CsvTextDelimiter
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Comma | `0` | Pembatas koma. |
| Semicolon | `1` | Pembatas titik koma. |
| Space | `2` | Pembatas spasi. |
| Tab | `3` | Pembatas tab. |

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


