---
title: "فئة SaveTemplateOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Saving.SaveTemplateOptions. تسمح بتحديد خيارات إضافية عند حفظ مشروع كقالب"
type: docs
weight: 2200
url: /ar/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

يسمح بتحديد خيارات إضافية عند حفظ المشروع كقالب.

```csharp
public class SaveTemplateOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إزالة جميع القيم الفعلية من قالب المشروع. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إزالة جميع القيم الأساسية من قالب المشروع. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إزالة جميع التكاليف الثابتة من قالب المشروع. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إزالة معدلات الموارد من قالب المشروع. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


