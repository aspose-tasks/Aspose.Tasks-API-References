---
title: "TaskBaseline.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskBaseline. تُرجع قيمة تشير إلى ما إذا كان هذا المثيل مساويًا لكائن TaskBaseline المحدد"
type: docs
weight: 100
url: /ar/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

يرجع قيمة تشير إلى ما إذا كانت هذه النسخة مساوية لكائن `TaskBaseline` المحدد.

```csharp
public bool Equals(TaskBaseline other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| آخر | TaskBaseline | كائن AssignmentBaseline المحدد للمقارنة مع هذه النسخة. |

### قيمة الإرجاع

تُرجع true إذا كان هذا المثيل مساويًا لكائن TaskBaseline المحدد؛ وإلا، false.

## الأمثلة

يعرض كيفية التحقق من مساواة الخطوط الأساسية.

```csharp
var project = new Project();

// إنشاء TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// عرض مدة TaskBaseline للمهمة
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// يتم التحقق من مساواة الخطوط الأساسية مقابل أرقام Baseline.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### انظر أيضًا

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_2}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

## الأمثلة

يعرض كيفية التحقق من مساواة الخطوط الأساسية.

```csharp
var project = new Project();

// إنشاء TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// عرض مدة TaskBaseline للمهمة
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// يتم التحقق من مساواة الخطوط الأساسية مقابل أرقام Baseline.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### انظر أيضًا

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


