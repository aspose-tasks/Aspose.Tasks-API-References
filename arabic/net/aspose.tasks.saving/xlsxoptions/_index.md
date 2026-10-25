---
title: "فئة XlsxOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Saving.XlsxOptions. تسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى XLSX"
type: docs
weight: 2270
url: /ar/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى XLSX.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | يُنشئ مثلاً جديداً من الفئة `XlsxOptions` التي يمكن استخدامها لحفظ المشروع بتنسيق XLSX. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | يحصل أو يعيّن قائمة بأعمدة عرض التعيينات التي سيتم عرضها ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | يحصل أو يضبط ترميز ملف XLSX الناتج. القيمة الافتراضية هي UTF8. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | يحصل أو يعيّن قائمة بأعمدة عرض الموارد التي سيتم عرضها ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | يحصل أو يعيّن التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | يحصل أو يعيّن المقارن لفرز المهام على مخطط جانت ومخطط ورقة المهام. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | يحصل أو يعيّن الشرط المستخدم لتصفية المهام المعروضة على مخططات جانت، ورقة المهام، واستخدام المهام. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | يحصل أو يضبط قائمة أعمدة العرض ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) لحفظها بتنسيق XLSX. إذا لم يتم الضبط فسيتم حفظ الأعمدة الافتراضية. |

## الأمثلة

يوضح كيفية حفظ مشروع في ملف XLSX باستخدام خيارات &lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// إضافة أعمدة مخطط جانت المطلوبة
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// إضافة أعمدة عرض الموارد المطلوبة
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// إضافة أعمدة عرض التعيينات المطلوبة
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// تعيين الترميز
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### انظر أيضًا

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


