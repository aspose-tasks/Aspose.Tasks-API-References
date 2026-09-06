---
title: "XlsxOptions.Encoding"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية XlsxOptions. يحصل أو يحدد ترميز ملف XLSX الناتج. القيمة الافتراضية هي UTF8"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/xlsxoptions/encoding/
---
## XlsxOptions.Encoding property

يحصل أو يضبط ترميز ملف XLSX الناتج. القيمة الافتراضية هي UTF8.

```csharp
public Encoding Encoding { get; set; }
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


