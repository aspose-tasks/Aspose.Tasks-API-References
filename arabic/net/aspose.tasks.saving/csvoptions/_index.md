---
title: "فئة CsvOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.Saving.CsvOptions فئة. يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى CSV"
type: docs
weight: 1980
url: /ar/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى CSV.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CsvOptions](csvoptions/)() | ينشئ مثيلاً جديدًا من فئة `CsvOptions` التي يمكن استخدامها لحفظ المشروع بصيغة CSV. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | يحصل أو يعيّن فئة البيانات التي سيتم حفظها. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | يحصل أو يعيّن ترميزًا لحفظ CSV به. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تضمين العناوين أم لا (القيمة الافتراضية هي TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | يحصل أو يعيّن التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | يحصل أو يعيّن المقارن لفرز المهام على مخطط جانت ومخطط ورقة المهام. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | يحصل أو يعيّن الشرط المستخدم لتصفية المهام المعروضة على مخططات جانت، ورقة المهام، واستخدام المهام. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | يحصل أو يضبط محدد النص. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | يحصل أو يضبط قائمة أعمدة العرض ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) لحفظها بتنسيق XLSX. إذا لم يتم الضبط فسيتم حفظ الأعمدة الافتراضية. |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


