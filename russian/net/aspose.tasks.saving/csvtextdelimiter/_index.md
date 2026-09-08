---
title: "Перечисление CsvTextDelimiter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Saving.CsvTextDelimiter. Разделитель текста для формата CSV"
type: docs
weight: 1990
url: /ru/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

Разделитель текста для формата CSV.

```csharp
public enum CsvTextDelimiter
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Comma | `0` | Разделитель — запятая. |
| Semicolon | `1` | Разделитель — точка с запятой. |
| Space | `2` | Разделитель — пробел. |
| Tab | `3` | Разделитель — табуляция. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


