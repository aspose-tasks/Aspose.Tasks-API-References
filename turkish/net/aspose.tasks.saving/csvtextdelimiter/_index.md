---
title: "CsvTextDelimiter enum'ı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.CsvTextDelimiter enum'ı. CSV formatı için metin sınırlayıcısı"
type: docs
weight: 1990
url: /tr/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

CSV formatı için metin ayırıcı.

```csharp
public enum CsvTextDelimiter
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Comma | `0` | Virgül sınırlayıcısı. |
| Semicolon | `1` | Noktalı virgül sınırlayıcısı. |
| Space | `2` | Boşluk sınırlayıcısı. |
| Tab | `3` | Sekme sınırlayıcısı. |

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


