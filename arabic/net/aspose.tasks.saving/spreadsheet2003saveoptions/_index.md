---
title: "الفئة Spreadsheet2003SaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Saving.Spreadsheet2003SaveOptions. تسمح بتحديد خيارات إضافية عند عرض صفحات المشروع إلى Spreadsheet2003"
type: docs
weight: 2220
url: /ar/net/aspose.tasks.saving/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions class

يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى Spreadsheet2003.

```csharp
public class Spreadsheet2003SaveOptions : SimpleSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Spreadsheet2003SaveOptions](spreadsheet2003saveoptions/)() | ينشئ مثيلاً جديداً للفئة `Spreadsheet2003SaveOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/) { get; set; } | يحصل أو يعيّن قائمة بأعمدة عرض التعيينات التي سيتم عرضها ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [ResourceView](../../aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/) { get; set; } | يحصل أو يعيّن قائمة بأعمدة عرض الموارد التي سيتم عرضها ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | يحصل أو يعيّن التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | يحصل أو يعيّن المقارن لفرز المهام على مخطط جانت ومخطط ورقة المهام. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | يحصل أو يعيّن الشرط المستخدم لتصفية المهام المعروضة على مخططات جانت، ورقة المهام، واستخدام المهام. |
| [View](../../aspose.tasks.saving/spreadsheet2003saveoptions/view/) { get; set; } | يحصل أو يعيّن قائمة بأعمدة العرض ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) التي سيتم حفظها. إذا لم يتم تعيينها فسيتم حفظ الأعمدة الافتراضية. |

## الأمثلة

يعرض كيفية إضافة أعمدة لتصديرها أثناء تصدير المشروع إلى تنسيق Spreadsheet2003.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### انظر أيضًا

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


