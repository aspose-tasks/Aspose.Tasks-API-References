---
title: "CsvOptions.CsvOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ CsvOptions. يهيئ نسخة جديدة من فئة CsvOptions التي يمكن استخدامها لحفظ المشروع بصيغة CSV"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

يهيئ نسخة جديدة من الفئة [`CsvOptions`](../) التي يمكن استخدامها لحفظ المشروع بصيغة CSV.

```csharp
public CsvOptions()
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


