---
title: "CsvOptions.CsvOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CsvOptions yapıcı. Projeyi CSV formatında kaydetmek için kullanılabilecek CsvOptions sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

Projeyi CSV formatında kaydetmek için kullanılabilecek [`CsvOptions`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public CsvOptions()
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


