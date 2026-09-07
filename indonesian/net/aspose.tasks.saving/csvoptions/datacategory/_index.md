---
title: "CsvOptions.DataCategory"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "CsvOptions properti. Mendapatkan atau mengatur kategori data yang akan disimpan"
type: docs
weight: 20
url: /id/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

Mendapatkan atau mengatur kategori data yang akan disimpan.

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


