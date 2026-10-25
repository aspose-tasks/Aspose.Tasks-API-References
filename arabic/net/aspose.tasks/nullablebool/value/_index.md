---
title: "NullableBool.Value"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية NullableBool. يحصل أو يعيّن قيمة تشير إلى ما إذا كانت القيمة الحالية true أو false"
type: docs
weight: 30
url: /ar/net/aspose.tasks/nullablebool/value/
---
## NullableBool.Value property

يحصل أو يعيّن قيمة تشير إلى ما إذا كانت القيمة الحالية صحيحة أم خاطئة.

```csharp
public bool Value { get; set; }
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


