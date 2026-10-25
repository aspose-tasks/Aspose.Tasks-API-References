---
title: "فئة ProjectView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Visualization.ProjectView. فئة عرض المشاريع"
type: docs
weight: 3300
url: /ar/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

فئة عرض المشروع

```csharp
public class ProjectView
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | ينشئ مثيلاً جديداً من فئة `ProjectView`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | يحصل على أعمدة عرض المشروع. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | يتضمن أعمدة UID، اسم المهمة، اسم المورد، العمل ومدة التعيين. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | يتضمن أعمدة المعرف، المؤشرات، الاسم، المدة، بدء وانتهاء المهمة. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | يتضمن أعمدة UID، اسم المورد، النوع، تسمية المادة، الأحرف الأولى، المجموعة، الحد الأقصى للوحدات، السعر القياسي، سعر العمل الإضافي، التكلفة لكل استخدام، تراكم عند، التقويم الأساسي وعمود رمز المورد. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | يتضمن أعمدة Uid والاسم والبداية والنهاية وموارد العمل. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | يتضمن أعمدة المهمة id والمؤشرات والاسم والمدة والبداية والنهاية والسابقين وأسماء الموارد. |

## الأمثلة

يوضح كيفية حفظ مشروع مع عرض التعيين.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


