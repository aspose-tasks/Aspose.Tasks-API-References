---
title: "CsvOptions.DataCategory"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CsvOptions özelliği. Kaydedilecek bir veri kategorisini alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

Kaydedilecek bir veri kategorisini alır veya ayarlar.

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


