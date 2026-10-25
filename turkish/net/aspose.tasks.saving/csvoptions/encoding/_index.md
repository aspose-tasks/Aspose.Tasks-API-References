---
title: "CsvOptions.Encoding"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CsvOptions özelliği. CSV'yi kaydetmek için bir kodlama alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

CSV'yi kaydetmek için bir kodlamayı alır veya ayarlar.

```csharp
public Encoding Encoding { get; set; }
```

## Örnekler

Bir projeyi CSV dosyası olarak kaydetmek için &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; kullanımını gösterir.

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

### Ayrıca Bakınız

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


