---
title: Enum DataCategory
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.DataCategory enum. The category of data used when saving to CSV
type: docs
weight: 1970
url: /net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

The category of data used when saving to CSV.

```csharp
public enum DataCategory
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Tasks | `0` | Tasks information. |
| Resources | `1` | Resources information. |
| Assignments | `2` | Assignments information. |

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


