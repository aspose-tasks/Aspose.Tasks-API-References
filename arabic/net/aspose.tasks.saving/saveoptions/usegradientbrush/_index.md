---
title: "SaveOptions.UseGradientBrush"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند عرض مخطط جانت"
type: docs
weight: 220
url: /ar/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند عرض مخطط جانت.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## ملاحظات

يُطبق فقط عندما يتم تصوير عرض مخطط Gantt.

## الأمثلة

يوضح كيفية ضبط قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند عرض مخطط جانت.

```csharp
var project = new Project(DataDir + "Project2.mpp");

SaveOptions options = new XamlOptions
{
    UseGradientBrush = false
};
project.Save(OutDir + "ChangeGanttBarsColorGradient_Solid_out.xaml", options);

options.UseGradientBrush = true;
project.Save(OutDir + "ChangeGanttBarsColorGradient_Gradient_out.xaml", options);
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


