---
title: "SaveTemplateOptions.RemoveBaselineValues"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveTemplateOptions. تحصل أو تعيين قيمة تشير إلى ما إذا كان يجب إزالة جميع قيم الخط الأساسي من قالب المشروع"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/savetemplateoptions/removebaselinevalues/
---
## SaveTemplateOptions.RemoveBaselineValues property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إزالة جميع القيم الأساسية من قالب المشروع.

```csharp
public bool RemoveBaselineValues { get; set; }
```

## الأمثلة

يوضح كيفية حفظ المشروع كقالب باستخدام الخيارات.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// إنشاء خيارات حفظ القالب
// وتعديل خصائصه
var options = new SaveTemplateOptions
{
    // تعيين قيمة تشير إلى ما إذا كان يجب إزالة جميع التكاليف الثابتة من قالب المشروع
    RemoveFixedCosts = true,

    // تعيين قيمة تشير إلى ما إذا كان يجب إزالة جميع القيم الفعلية من قالب المشروع
    RemoveActualValues = true,

    // تعيين قيمة تشير إلى ما إذا كان يجب إزالة معدلات الموارد من قالب المشروع
    RemoveResourceRates = true,

    // تعيين قيمة تشير إلى ما إذا كان يجب إزالة جميع القيم الأساسية من قالب المشروع
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### انظر أيضًا

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


