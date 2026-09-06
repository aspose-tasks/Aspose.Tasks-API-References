---
title: "ResourceAssignment.Set"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تُطابق الخاصية المحددة مع القيمة المحددة في هذه الحاوية"
type: docs
weight: 750
url: /ar/net/aspose.tasks/resourceassignment/set/
---
## ResourceAssignment.Set&lt;T&gt; method

يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

```csharp
public void Set<T>(Key<T, AsnKey> key, T val)
```

| معامل | الوصف |
| --- | --- |
| T | نوع القيمة المرتبطة. |
| key | مفتاح الخاصية المحدد. [`Asn`](../../asn/) للحصول على مفتاح الخاصية. |
| القيمة | القيمة. |

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


