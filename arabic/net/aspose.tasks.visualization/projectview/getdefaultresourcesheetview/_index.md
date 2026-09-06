---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectView. تشمل أعمدة Uid واسم المورد type وmaterial وlabel وinitials وgroup وmax units وstandard rate وovertime rate وcost per use وaccrue at وbase calendar وcode"
type: docs
weight: 40
url: /ar/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

يتضمن أعمدة UID، اسم المورد، النوع، تسمية المادة، الأحرف الأولى، المجموعة، الحد الأقصى للوحدات، السعر القياسي، سعر العمل الإضافي، التكلفة لكل استخدام، تراكم عند، التقويم الأساسي وعمود رمز المورد.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### قيمة الإرجاع

عرض يحتوي على قائمة بـ [`ResourceViewColumn`](../../resourceviewcolumn/).

## الأمثلة

يوضح كيفية حفظ مشروع مع عرض ورقة الموارد.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### انظر أيضًا

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


