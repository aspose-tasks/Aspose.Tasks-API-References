---
title: "CsvOptions.IncludeHeaders"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CsvOptions. تحصل أو تعيّن قيمة تشير إلى ما إذا كان يجب تضمين العناوين أم لا؛ القيمة الافتراضية هي TRUE"
type: docs
weight: 40
url: /ar/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تضمين العناوين أم لا (القيمة الافتراضية هي TRUE).

```csharp
public bool IncludeHeaders { get; set; }
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


