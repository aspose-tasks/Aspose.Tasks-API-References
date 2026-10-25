---
title: "XlsxOptions.XlsxOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ XlsxOptions. يهيئ نسخة جديدة من فئة XlsxOptions التي يمكن استخدامها لحفظ المشروع بصيغة XLSX"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/xlsxoptions/xlsxoptions/
---
## XlsxOptions constructor

يهيئ نسخة جديدة من الفئة [`XlsxOptions`](../) التي يمكن استخدامها لحفظ المشروع بصيغة XLSX.

```csharp
public XlsxOptions()
```

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

* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


