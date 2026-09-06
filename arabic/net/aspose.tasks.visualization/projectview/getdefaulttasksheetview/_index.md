---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectView. تتضمن أعمدة المهمة التي تشمل المعرف والمؤشرات والاسم والمدة والبداية والنهاية والسلف وأسماء الموارد"
type: docs
weight: 60
url: /ar/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

يتضمن أعمدة المهمة id والمؤشرات والاسم والمدة والبداية والنهاية والسابقين وأسماء الموارد.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### قيمة الإرجاع

عرض يحتوي على قائمة من [`GanttChartColumn`](../../ganttchartcolumn/).

## الأمثلة

يوضح كيفية حفظ مشروع مع عرض ورقة المهام.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### انظر أيضًا

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


