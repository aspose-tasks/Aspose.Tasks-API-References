---
title: "SaveOptions.RenderToSinglePage"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب تصوير المشروع في صفحة واحدة عندما يتم حفظ المشروع بصيغة رسومية. سيتم تغيير حجم الصفحة بحيث يمكن أن يتناسب المشروع المصور على صفحة واحدة"
type: docs
weight: 150
url: /ar/net/aspose.tasks.saving/saveoptions/rendertosinglepage/
---
## SaveOptions.RenderToSinglePage property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب عرض المشروع في صفحة واحدة عندما يُحفظ المشروع بصيغة رسومية. سيتم تغيير حجم الصفحة بحيث يتناسب المشروع المعروض على صفحة واحدة.

```csharp
public bool RenderToSinglePage { get; set; }
```

## الأمثلة

يوضح كيفية حفظ الصفحات المختارة لمشروع في ملف PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// دعنا نتحقق من عدد الصفحات التي يمكن تصديرها
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

يوضح كيفية استخدام خاصية RenderToSinglePage لتحديد أن المشروع يجب أن يُحفظ كملف PDF من صفحة واحدة.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.TaskUsage;
options.Timescale = Timescale.DefinedInView;
options.RenderToSinglePage = true;
options.StartDate = new DateTime(2012, 12, 22);
options.EndDate = new DateTime(2013, 05, 10);

project.Save(OutDir + "WorkWithRenderToSinglePage_out.pdf", options);
```

يوضح كيفية حفظ الصفحات المحددة كصورة.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

يوضح كيفية حفظ التخطيط إلى ملفات منفصلة.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.FontSettings.DefaultFontName = "Segoe UI Black";
options.FontSettings.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// احفظ تخطيط المشروع إلى ملفات منفصلة
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


