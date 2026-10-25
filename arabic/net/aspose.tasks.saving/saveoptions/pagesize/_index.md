---
title: "SaveOptions.PageSize"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يضبط حجم الصفحة التي سيتم عرضها القيمة الافتراضية هي PageSize.A4"
type: docs
weight: 130
url: /ar/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

يحصل أو يعيّن حجم الصفحة التي سيتم عرضها (القيمة الافتراضية هي PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## الأمثلة

يوضح كيفية ضبط حجم الصفحة (يمكن أن يكون أحد قيم التعداد &lt;see cref="P:Aspose.Tasks.Visualization.TiffCompression" /&gt;).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// عرض المشروع بجميع أحجام الصفحات المعرفة مسبقًا
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### انظر أيضًا

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


