---
title: "SaveOptions.FitContent"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف لتناسب محتواه."
type: docs
weight: 50
url: /ar/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه.

```csharp
public bool FitContent { get; set; }
```

## الأمثلة

يعرض كيفية ضبط الخيار لتحديد ما إذا كان يجب زيادة ارتفاع الصف ليتناسب مع محتواه.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // ضبط خيار ملاءمة المحتوى إلى true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


