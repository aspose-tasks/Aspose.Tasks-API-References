---
title: "CsvOptions.TextDelimiter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti CsvOptions. Mendapatkan atau mengatur pembatas teks"
type: docs
weight: 50
url: /id/net/aspose.tasks.saving/csvoptions/textdelimiter/
---
## CsvOptions.TextDelimiter property

Mendapatkan atau mengatur pembatas teks.

```csharp
public CsvTextDelimiter TextDelimiter { get; set; }
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

* enum [CsvTextDelimiter](../../csvtextdelimiter/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


