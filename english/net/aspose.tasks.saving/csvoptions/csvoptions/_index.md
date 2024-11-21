---
title: CsvOptions.CsvOptions
second_title: Aspose.Tasks for .NET API Reference
description: CsvOptions constructor. Initializes a new instance of the CsvOptions class which can be used to save project in CSV format
type: docs
weight: 10
url: /net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

Initializes a new instance of the [`CsvOptions`](../) class which can be used to save project in CSV format.

```csharp
public CsvOptions()
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


