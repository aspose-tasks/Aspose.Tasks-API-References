---
title: "CsvOptions.Encoding"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CsvOptions. يحصل أو يضبط ترميزًا لحفظ CSV به"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

يحصل أو يعيّن ترميزًا لحفظ CSV به.

```csharp
public Encoding Encoding { get; set; }
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

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


