---
title: CsvOptions.DataCategory
second_title: Aspose.Tasks for .NET API Reference
description: CsvOptions property. Gets or sets a data category to be saved
type: docs
weight: 20
url: /net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

Gets or sets a data category to be saved.

```csharp
public DataCategory DataCategory { get; set; }
```

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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


