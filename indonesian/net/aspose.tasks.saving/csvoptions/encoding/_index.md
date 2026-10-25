---
title: "CsvOptions.Encoding"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti CsvOptions. Mendapatkan atau mengatur encoding untuk menyimpan CSV"
type: docs
weight: 30
url: /id/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

Mendapatkan atau mengatur enkoding untuk menyimpan CSV.

```csharp
public Encoding Encoding { get; set; }
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


