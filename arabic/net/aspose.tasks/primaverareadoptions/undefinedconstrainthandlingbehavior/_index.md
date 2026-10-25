---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PrimaveraReadOptions. تحدد السلوك المستخدم لمعالجة المهام ذات القيود غير المحددة المقروءة من تنسيق XER"
type: docs
weight: 50
url: /ar/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

يحدد السلوك المستخدم لمعالجة المهام ذات القيود غير المعرفة المقروءة من تنسيق XER.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


