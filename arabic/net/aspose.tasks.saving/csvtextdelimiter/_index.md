---
title: "تعداد CsvTextDelimiter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Saving.CsvTextDelimiter. محدد النص لتنسيق CSV"
type: docs
weight: 1990
url: /ar/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

فاصل النص لتنسيق CSV.

```csharp
public enum CsvTextDelimiter
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Comma | `0` | محدد الفاصلة (،). |
| Semicolon | `1` | محدد الفاصلة المنقوطة (؛). |
| Space | `2` | محدد الفراغ. |
| Tab | `3` | محدد علامة الجدولة. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


