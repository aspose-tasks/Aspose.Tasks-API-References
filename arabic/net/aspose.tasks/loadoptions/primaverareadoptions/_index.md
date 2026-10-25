---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعيّن نسخة محددة من فئة PrimaveraReadOptions التي يمكن استخدامها لتخصيص سلوك تحميل صيغ Primavera مثل Primavera P6 XER أو Primavera P6 Xml"
type: docs
weight: 60
url: /ar/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

تحصل أو تعيّن نسخة محددة من الفئة [`PrimaveraReadOptions`](../../primaverareadoptions/) التي يمكن استخدامها لتخصيص سلوك تحميل صيغ Primavera (Primavera P6 XER أو Primavera P6 Xml).

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
```

## الأمثلة

يوضح كيفية تحميل مشروع Primavera بالمعرف المحدد باستخدام &lt;see cref="LoadOptions" /&gt;.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// تعيين خيارات قراءة Primavera
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// العمل مع المشروع...
```

### انظر أيضًا

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


