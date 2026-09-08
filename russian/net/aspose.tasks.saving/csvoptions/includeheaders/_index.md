---
title: "CsvOptions.IncludeHeaders"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CsvOptions. Возвращает или задает значение, указывающее, включать ли заголовки; значение по умолчанию — TRUE."
type: docs
weight: 40
url: /ru/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

Получает или задает значение, указывающее, включать ли заголовки (значение по умолчанию — TRUE).

```csharp
public bool IncludeHeaders { get; set; }
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


