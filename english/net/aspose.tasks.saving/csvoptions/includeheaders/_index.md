---
title: CsvOptions.IncludeHeaders
second_title: Aspose.Tasks for .NET API Reference
description: CsvOptions property. Gets or sets a value indicating whether to include headers or not default value is TRUE
type: docs
weight: 40
url: /net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

Gets or sets a value indicating whether to include headers or not (default value is TRUE).

```csharp
public bool IncludeHeaders { get; set; }
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

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


