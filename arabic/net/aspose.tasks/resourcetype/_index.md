---
title: "تعداد ResourceType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.ResourceType. يحدد نوع المورد"
type: docs
weight: 1800
url: /ar/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

يحدد نوع المورد.

```csharp
public enum ResourceType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Material | `0` | يشير إلى نوع المورد المادي. |
| Work | `1` | يشير إلى نوع المورد العمل. |
| Cost | `2` | يشير إلى نوع المورد التكلفة. |

## الأمثلة

يوضح كيفية العمل مع أنواع الموارد.

```csharp
var project = new Project();

// إضافة مورد عمل
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// إضافة مورد مادي
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// إضافة مورد مادي
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// العمل مع الموارد: إنشاء مهام، تعيين موارد، وما إلى ذلك...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


