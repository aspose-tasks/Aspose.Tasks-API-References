---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectView. تتضمن أعمدة المهمة التي تشمل المعرف والمؤشرات والاسم والمدة والبداية والنهاية"
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

يتضمن أعمدة المعرف، المؤشرات، الاسم، المدة، بدء وانتهاء المهمة.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### قيمة الإرجاع

عرض يحتوي على قائمة من [`GanttChartColumn`](../../ganttchartcolumn/).

## الأمثلة

يوضح كيفية حفظ مشروع مع عرض مخطط جانت.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### انظر أيضًا

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


