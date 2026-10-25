---
title: "تعداد DataCategory"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Saving.DataCategory. فئة البيانات المستخدمة عند الحفظ إلى CSV."
type: docs
weight: 2000
url: /ar/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

فئة البيانات المستخدمة عند الحفظ إلى CSV.

```csharp
public enum DataCategory
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Tasks | `0` | معلومات المهام. |
| Resources | `1` | معلومات الموارد. |
| Assignments | `2` | معلومات التعيينات. |

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


