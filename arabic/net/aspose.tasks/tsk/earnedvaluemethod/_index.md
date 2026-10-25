---
title: "Tsk.EarnedValueMethod"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كان يجب استخدام حقل  Complete أو Physical  Complete لحساب التكلفة المقدرة للعمل المنجز BCWP."
type: docs
weight: 350
url: /ar/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

يحدد ما إذا كان يجب استخدام حقل % المكتمل أو % المكتمل الفعلي لحساب التكلفة الموازنة للعمل المنفذ (BCWP).

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Tsk.EarnedValueMethod.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


