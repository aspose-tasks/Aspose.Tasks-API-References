---
title: "TaskBaseline.CompareTo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskBaseline. تنفيذ واجهة IComparable. يقارن هذا المثيل بالكيان Baseline المحدد"
type: docs
weight: 90
url: /ar/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

تنفيذ واجهة IComparable. يقارن هذه الحالة بالكائن Baseline المحدد.

```csharp
public int CompareTo(TaskBaseline other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| آخر | TaskBaseline | الكيان Baseline المحدد للمقارنة مع هذه الحالة. |

### قيمة الإرجاع

يرجع -1 إذا كانت هذه الحالة أصغر من الكائن المحدد، 1 إذا كانت هذه الحالة أكبر من الكائن المحدد؛ وإلا يرجع 0

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


