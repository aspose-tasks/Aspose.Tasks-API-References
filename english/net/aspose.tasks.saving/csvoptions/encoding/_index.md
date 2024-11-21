---
title: CsvOptions.Encoding
second_title: Aspose.Tasks for .NET API Reference
description: CsvOptions property. Gets or sets an encoding to save CSV with
type: docs
weight: 30
url: /net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

Gets or sets an encoding to save CSV with.

```csharp
public Encoding Encoding { get; set; }
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


