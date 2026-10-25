---
title: "هيكل NullableBool."
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "هيكل Aspose.Tasks.NullableBool. فئة للقيم البوليانية مع إمكانية التحقق مما إذا كانت القيمة معرفة أم لا."
type: docs
weight: 1110
url: /ar/net/aspose.tasks/nullablebool/
---
## NullableBool structure

فئة للقيم المنطقية مع إمكانية التحقق مما إذا كانت القيمة معرفة أم لا.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | يُنشئ نسخة جديدة من هيكل `NullableBool` بالقيمة البوليانية المحددة. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | يُنشئ نسخة جديدة من هيكل `NullableBool`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت القيمة معرفة؛ وإلا، false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت القيمة الحالية صحيحة أم خاطئة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | يرجع علامة تشير إلى ما إذا كانت هذه النسخة مساوية للنسخة المحددة من الفئة `NullableBool`. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | يرجع علامة تشير إلى ما إذا كانت هذه المثيلة مساوية للعنصر المحدد. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | يرجع قيمة رمز تجزئة للنسخة من الفئة `NullableBool`. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | يرجع سلسلة تمثل الكائن الحالي. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | يقوم بتحويل كائن `NullableBool` إلى قيمة منطقية ضمنيًا. يرجع true عندما يكون [`Value`](./value/) true و[`IsDefined`](./isdefined/) true. (2 عمليات) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


