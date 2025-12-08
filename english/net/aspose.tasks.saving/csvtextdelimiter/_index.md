---
title: Enum CsvTextDelimiter
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.CsvTextDelimiter enum. Text delimiter for CSV format
type: docs
weight: 1960
url: /net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

Text delimiter for CSV format.

```csharp
public enum CsvTextDelimiter
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Comma | `0` | Comma delimiter. |
| Semicolon | `1` | Semicolon delimiter. |
| Space | `2` | Space delimiter. |
| Tab | `3` | Tab delimiter. |

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; to save a project as CSV file.

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

### See Also

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


