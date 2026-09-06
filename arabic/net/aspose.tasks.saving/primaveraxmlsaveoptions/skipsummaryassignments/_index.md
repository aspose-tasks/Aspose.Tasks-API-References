---
title: "PrimaveraXmlSaveOptions.SkipSummaryAssignments"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PrimaveraXmlSaveOptions. تحصل أو تعيين قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى المهام الملخصة أثناء التصدير"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/
---
## PrimaveraXmlSaveOptions.SkipSummaryAssignments property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى المهام الملخصة أثناء التصدير.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## ملاحظات

لا يدعم برنامج Primavera تعيينات الموارد إلى المهام الملخصة (WBS). وبالتالي، قد يؤدي تصدير هذه التعيينات إلى ملف غير صالح وفقًا لنموذج Primavera. إذا كانت القيمة true، يتم تخطي التعيينات إلى المهام الملخصة أثناء التصدير. إذا كانت false (القيمة الافتراضية)، سيتم رمي استثناء إذا تم مواجهة تعيين إلى مهمة ملخصة أثناء التصدير.

## الأمثلة

يوضح كيفية استخدام علم SkipSummaryAssignments.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// لا يدعم Primavera تعيينات الموارد إلى المهام الملخصة.
// لذلك قد يؤدي تصدير هذه التعيينات إلى تنسيق Primavera إلى ملفات لا يمكن استيرادها إلى Primavera.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### انظر أيضًا

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


