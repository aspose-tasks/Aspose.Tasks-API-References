---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PrimaveraReadOptions. تحصل أو تعيّن علامة تحدد ما إذا كان يجب الحفاظ على المعرفات الفريدة الأصلية للكيانات"
type: docs
weight: 20
url: /ar/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

يحصل أو يضبط علامة تحدد ما إذا كان يجب الحفاظ على المعرفات الفريدة الأصلية للكيانات.

```csharp
public bool PreserveUids { get; set; }
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

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


