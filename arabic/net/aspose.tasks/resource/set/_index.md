---
title: "Resource.Set"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Resource. تقوم بربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية"
type: docs
weight: 860
url: /ar/net/aspose.tasks/resource/set/
---
## Set&lt;T&gt;(Key&lt;T, RscKey&gt;, T) {#set_1}

يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

```csharp
public void Set<T>(Key<T, RscKey> key, T val)
```

| معامل | الوصف |
| --- | --- |
| T | نوع القيمة المرتبطة. |
| key | مفتاح الخاصية المحدد. [`Rsc`](../../rsc/) للحصول على مفتاح الخاصية. |
| القيمة | القيمة. |

## الأمثلة

يوضح كيفية قراءة/كتابة خصائص الموارد الشائعة.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// أضف موردًا واضبط بعض الخصائص
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, RscKey&gt;, DateTime) {#set}

يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

```csharp
public void Set(Key<DateTime, RscKey> key, DateTime val)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| key | Key`2 | مفتاح الخاصية المحدد. [`Rsc`](../../rsc/) للحصول على مفتاح الخاصية. |
| القيمة | DateTime | القيمة. |

## الأمثلة

يوضح كيفية قراءة/كتابة خصائص الموارد الشائعة.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// أضف موردًا واضبط بعض الخصائص
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


