---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة FieldHelper. تُرجع عنوانًا افتراضيًا للحقل المحدد"
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

تُعيد عنوانًا افتراضيًا للحقل المحدد.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| حقل | حقل | حقل للحصول على عنوان افتراضي. |

### قيمة الإرجاع

عنوان افتراضي للحقل المحدد إذا كان يمكن عرض الحقل في عرض MS Project، وإلا يكون null.

## الأمثلة

يوضح كيفية استخدام &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; لأخذ أعمدة مخطط جانت الافتراضي و

```csharp
// احفظها في ملف CSV.
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### انظر أيضًا

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


