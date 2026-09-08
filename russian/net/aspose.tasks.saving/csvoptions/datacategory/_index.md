---
title: "CsvOptions.DataCategory"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CsvOptions. Возвращает или задает категорию данных для сохранения."
type: docs
weight: 20
url: /ru/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

Получает или задает категорию данных для сохранения.

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


