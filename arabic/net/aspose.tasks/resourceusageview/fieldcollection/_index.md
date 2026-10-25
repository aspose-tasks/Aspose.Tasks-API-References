---
title: "ResourceUsageView.FieldCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ResourceUsageView. تحصل على كائن ResourceUsageViewFieldCollection لهذا الـ ResourceUsageView."
type: docs
weight: 10
url: /ar/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

تحصل على كائن [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) لهذا الـ ResourceUsageView.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## الأمثلة

يعرض كيفية قراءة حقول عرض استخدام الموارد.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### انظر أيضًا

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


