---
title: "NullableBool.NullableBool"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ NullableBool. يهيئ كائنًا جديدًا من بنية NullableBool بالقيمة المنطقية المحددة."
type: docs
weight: 10
url: /ar/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

يهيئ كائنًا جديدًا من بنية [`NullableBool`](../) بالقيمة المنطقية المحددة.

```csharp
public NullableBool(bool value)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| value | Boolean | القيمة المنطقية المحددة. |

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

---

## NullableBool(bool, bool) {#constructor_1}

يُنشئ مثيلاً جديدًا من بنية [`NullableBool`](../).

```csharp
public NullableBool(bool value, bool isDefined)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| value | Boolean | القيمة الحالية. |
| isDefined | Boolean | القيمة التي تشير إلى ما إذا كانت القيمة الحالية معرفة. |

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


