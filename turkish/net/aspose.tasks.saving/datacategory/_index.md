---
title: "Enum DataCategory"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.DataCategory enum. CSV'ye kaydedilirken kullanılan veri kategorisini belirtir."
type: docs
weight: 2000
url: /tr/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

CSV'ye kaydedilirken kullanılan veri kategorisi.

```csharp
public enum DataCategory
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Tasks | `0` | Görevler bilgisi. |
| Resources | `1` | Kaynaklar bilgisi. |
| Assignments | `2` | Atamalar bilgisi. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


