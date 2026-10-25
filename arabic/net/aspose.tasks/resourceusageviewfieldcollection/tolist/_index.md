---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceUsageViewFieldCollection. تُحوِّل نسخة من فئة ResourceUsageViewFieldCollection إلى قائمة تحتوي على نسخ من فئة ResourceUsageViewField"
type: docs
weight: 20
url: /ar/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

يحوِّل نسخة من فئة [`ResourceUsageViewFieldCollection`](../) إلى قائمة تحتوي على نسخ من فئة [`ResourceUsageViewField`](../../resourceusageviewfield/) .

```csharp
public IList<ResourceUsageViewField> ToList()
```

### قيمة الإرجاع

نسخة فئة [`ResourceUsageViewFieldCollection`](../) تم تحويلها إلى قائمة تحتوي على نسخ من فئة [`ResourceUsageViewField`](../../resourceusageviewfield/) .

## الأمثلة

يعرض كيفية التعامل مع مجموعة الحقول لنسخة من ResourceUsageView.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// يمكن تحويل المجموعة إلى قائمة من ResourceUsageViewField
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### انظر أيضًا

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


