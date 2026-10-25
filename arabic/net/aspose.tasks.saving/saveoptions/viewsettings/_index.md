---
title: "SaveOptions.ViewSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد عرض View للتصوير. يمكنك استخدام هذه الخيارات لتحديد بشكل صريح أي عرض يجب حفظه بصيغة PDF أو HTML أو Image. إذا تم تعيين هذه الخاصية، يتم تجاهل خاصية PresentationFormat عند حفظ المشروع. يجب أن يكون العرض من أحد الشاشات التالية: Screen, Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage."
type: docs
weight: 240
url: /ar/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

يحصل أو يحدد عرضًا ([`View`](../view/)) للتصوير. يمكنك استخدام هذه الخيارات لتحديد بشكل صريح أي عرض يجب حفظه بصيغة PDF أو HTML أو Image. إذا تم تعيين هذه الخاصية، يتم تجاهل خاصية [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) عند حفظ المشروع. يجب أن يكون العرض من أحد الشاشات التالية (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

```csharp
public View ViewSettings { get; set; }
```

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | عند استدعاء طريقة set وتوفير مثال من فئة View بقيمة غير مدعومة لخاصية Screen. |

## الأمثلة

يوضح كيفية استخدام 'SaveOptions.ViewSettings' لتحديد العرض الذي يجب تصويره إلى PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### انظر أيضًا

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


