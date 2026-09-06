---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. تحصل أو تعين لون الوقت غير العامل"
type: docs
weight: 110
url: /ar/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

يحصل أو يعيّن لون وقت عدم العمل.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## الأمثلة

يوضح كيفية تعيين لون مخصص للوقت غير العامل.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


