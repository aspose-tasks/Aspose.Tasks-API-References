---
title: "Resource.Get"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Resource. تُعيد القيمة التي تم تعيين الخاصية إليها في هذا الحاوية"
type: docs
weight: 830
url: /ar/net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية.

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| معامل | الوصف |
| --- | --- |
| T | نوع القيمة المرتبطة. |
| key | مفتاح الخاصية المحدد. [`Rsc`](../../rsc/) للحصول على مفتاح الخاصية. |

### قيمة الإرجاع

القيمة التي تم تعيين الخاصية إليها في هذا الحاوية.

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


