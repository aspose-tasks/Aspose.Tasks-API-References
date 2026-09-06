---
title: "تعداد WorkGroupType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.WorkGroupType. يحدد نوع مجموعة العمل"
type: docs
weight: 3620
url: /ar/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

يحدد نوع مجموعة العمل.

```csharp
public enum WorkGroupType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | يشير إلى نوع مجموعة العمل الافتراضية. |
| None | `1` | يشير إلى نوع مجموعة العمل 'None'. |
| Email | `2` | يشير إلى نوع مجموعة العمل البريد الإلكتروني. |
| Web | `3` | يشير إلى نوع مجموعة العمل الويب. |

## الأمثلة

يوضح كيفية تعيين مجموعة عمل لمورد.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


