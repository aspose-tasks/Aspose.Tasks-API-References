---
title: "NullableBool.ToString"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة NullableBool. تُعيد سلسلة تمثل الكائن الحالي."
type: docs
weight: 60
url: /ar/net/aspose.tasks/nullablebool/tostring/
---
## NullableBool.ToString method

يرجع سلسلة تمثل الكائن الحالي.

```csharp
public override string ToString()
```

### قيمة الإرجاع

سلسلة تمثل الكائن الحالي.

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


