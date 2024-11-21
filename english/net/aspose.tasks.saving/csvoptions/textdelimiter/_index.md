---
title: CsvOptions.TextDelimiter
second_title: Aspose.Tasks for .NET API Reference
description: CsvOptions property. Gets or sets a text delimiter
type: docs
weight: 50
url: /net/aspose.tasks.saving/csvoptions/textdelimiter/
---
## CsvOptions.TextDelimiter property

Gets or sets a text delimiter.

```csharp
public CsvTextDelimiter TextDelimiter { get; set; }
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

* enum [CsvTextDelimiter](../../csvtextdelimiter/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


