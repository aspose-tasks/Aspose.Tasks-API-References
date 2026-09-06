---
title: "CsvOptions.DataCategory"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CsvOptions. تحصل أو تعيّن فئة البيانات التي سيتم حفظها"
type: docs
weight: 20
url: /ar/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

يحصل أو يعيّن فئة البيانات التي سيتم حفظها.

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


