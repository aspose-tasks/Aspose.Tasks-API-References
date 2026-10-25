---
title: "TaskLink.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskLink. تُرجع قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية لكائن محدد"
type: docs
weight: 90
url: /ar/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public bool Equals(TaskLink other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| other | TaskLink | المثيل المحدد من الفئة [`TaskLink`](../) للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## الأمثلة

يظهر كيفية التحقق من مساواة روابط المهام.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// مساواة روابط المهام تستند إلى المهام السابقة واللاحقة.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### انظر أيضًا

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## الأمثلة

يظهر كيفية التحقق من مساواة روابط المهام.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// مساواة روابط المهام تستند إلى المهام السابقة واللاحقة.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### انظر أيضًا

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


