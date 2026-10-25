---
title: "CsvOptions.CsvOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor CsvOptions. Menginisialisasi instance baru dari kelas CsvOptions yang dapat digunakan untuk menyimpan proyek dalam format CSV"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

Menginisialisasi instance baru dari kelas [`CsvOptions`](../) yang dapat digunakan untuk menyimpan proyek dalam format CSV.

```csharp
public CsvOptions()
```

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

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


