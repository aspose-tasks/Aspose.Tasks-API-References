---
title: "ResourceAssignment.Get"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تُرجع القيمة التي تم ربط الخاصية بها في هذه الحاوية"
type: docs
weight: 700
url: /ar/net/aspose.tasks/resourceassignment/get/
---
## ResourceAssignment.Get&lt;T&gt; method

يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية.

```csharp
public T Get<T>(Key<T, AsnKey> key)
```

| معامل | الوصف |
| --- | --- |
| T | نوع القيمة المرتبطة. |
| key | مفتاح الخاصية المحدد. [`Asn`](../../asn/) للحصول على مفتاح الخاصية. |

### قيمة الإرجاع

القيمة التي تم تعيين الخاصية إليها في هذا الحاوية.

## الأمثلة

يوضح كيفية إنشاء تعيين والحصول على/تعيين خصائص التعيين العامة.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


