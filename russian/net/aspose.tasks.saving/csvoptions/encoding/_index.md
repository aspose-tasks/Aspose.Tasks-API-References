---
title: "CsvOptions.Encoding"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CsvOptions. Получает или задает кодировку для сохранения CSV"
type: docs
weight: 30
url: /ru/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

Получает или задает кодировку, с которой сохраняется CSV.

```csharp
public Encoding Encoding { get; set; }
```

## Примеры

Показывает, как использовать &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; для сохранения проекта в виде CSV-файла.

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

### См. также

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


