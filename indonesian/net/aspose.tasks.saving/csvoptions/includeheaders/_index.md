---
title: "CsvOptions.IncludeHeaders"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "CsvOptions properti. Mendapatkan atau mengatur nilai yang menunjukkan apakah menyertakan header atau tidak; nilai default adalah TRUE"
type: docs
weight: 40
url: /id/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

Mendapatkan atau mengatur nilai yang menunjukkan apakah menyertakan header atau tidak (nilai default adalah TRUE).

```csharp
public bool IncludeHeaders { get; set; }
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


