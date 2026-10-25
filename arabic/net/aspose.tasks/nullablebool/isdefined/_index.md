---
title: "NullableBool.IsDefined"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية NullableBool. تحصل على قيمة تشير إلى ما إذا كانت القيمة معرفة وإلا تكون false."
type: docs
weight: 20
url: /ar/net/aspose.tasks/nullablebool/isdefined/
---
## NullableBool.IsDefined property

يحصل على قيمة تشير إلى ما إذا كانت القيمة معرفة؛ وإلا، false.

```csharp
public bool IsDefined { get; }
```

## الأمثلة

يوضح كيفية العمل مع الفئة &lt;see cref=\"NullableBool\" /&gt;.

```csharp
var project = new Project();

// دعنا نتحقق من مكان استخدام الفئة <see cref=\"Aspose.Tasks.NullableBool\" />.
// الميزة الرئيسية لـ <see cref=\"Aspose.Tasks.NullableBool\" /> هي 
// يمكن تعيينه كغير معرف من خلال الإنشاء
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// استخدام كائن nullable bool
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// استخدام كائن nullable bool
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### انظر أيضًا

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


