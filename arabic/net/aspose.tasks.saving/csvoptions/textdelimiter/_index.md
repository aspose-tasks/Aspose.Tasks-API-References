---
title: "CsvOptions.TextDelimiter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CsvOptions. يحصل أو يضبط محدد النص"
type: docs
weight: 50
url: /ar/net/aspose.tasks.saving/csvoptions/textdelimiter/
---
## CsvOptions.TextDelimiter property

يحصل أو يضبط محدد النص.

```csharp
public CsvTextDelimiter TextDelimiter { get; set; }
```

## الأمثلة

يعرض كيفية استخدام &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; لحفظ مشروع كملف CSV.

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

### انظر أيضًا

* enum [CsvTextDelimiter](../../csvtextdelimiter/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


