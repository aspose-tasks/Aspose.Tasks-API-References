---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectView. تتضمن أعمدة الموارد التي تشمل المعرف الفريد والاسم والبداية والنهاية والعمل"
type: docs
weight: 50
url: /ar/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

يتضمن أعمدة Uid والاسم والبداية والنهاية وموارد العمل.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### قيمة الإرجاع

عرض يحتوي على قائمة بـ [`ResourceViewColumn`](../../resourceviewcolumn/).

## الأمثلة

يوضح كيفية حفظ مشروع مع عرض استخدام الموارد.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### انظر أيضًا

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


