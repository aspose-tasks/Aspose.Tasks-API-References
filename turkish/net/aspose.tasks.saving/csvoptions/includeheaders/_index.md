---
title: "CsvOptions.IncludeHeaders"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CsvOptions özelliği. Başlıkların dahil edilip edilmeyeceğini belirten bir değeri alır veya ayarlar; varsayılan değer TRUE'dur."
type: docs
weight: 40
url: /tr/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

Başlıkların dahil edilip edilmeyeceğini gösteren bir değeri alır veya ayarlar (varsayılan değer TRUE'dır).

```csharp
public bool IncludeHeaders { get; set; }
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


