---
title: "Перечисление DataCategory"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Saving.DataCategory. Категория данных, используемых при сохранении в CSV."
type: docs
weight: 2000
url: /ru/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

Категория данных, используемых при сохранении в CSV.

```csharp
public enum DataCategory
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Tasks | `0` | Информация о задачах. |
| Resources | `1` | Информация о ресурсах. |
| Assignments | `2` | Информация о назначениях. |

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


