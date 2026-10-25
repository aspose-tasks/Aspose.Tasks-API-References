---
title: "CsvOptions.CsvOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор CsvOptions. Инициализирует новый экземпляр класса CsvOptions, который можно использовать для сохранения проекта в формате CSV"
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

Инициализирует новый экземпляр класса [`CsvOptions`](../), который можно использовать для сохранения проекта в формате CSV.

```csharp
public CsvOptions()
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


