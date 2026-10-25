---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectView. تشمل أعمدة Uid واسم المهمة واسم المورد والعمل والمدة"
type: docs
weight: 20
url: /ar/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

يتضمن أعمدة UID، اسم المهمة، اسم المورد، العمل ومدة التعيين.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### قيمة الإرجاع

عرض يحتوي على قائمة بـ [`AssignmentViewColumn`](../../assignmentviewcolumn/).

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

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


