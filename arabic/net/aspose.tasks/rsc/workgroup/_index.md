---
title: "Rsc.Workgroup"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. نوع مجموعة العمل التي ينتمي إليها المورد"
type: docs
weight: 700
url: /ar/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

نوع مجموعة العمل التي ينتمي إليها المورد.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.Workgroup.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


