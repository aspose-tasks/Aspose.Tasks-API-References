---
title: "Class ResourceUsageViewFieldCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.ResourceUsageViewFieldCollection class. تمثّل مجموعة من قيم ResourceUsageViewField"
type: docs
weight: 1830
url: /ar/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

تمثّل مجموعة من قيم [`ResourceUsageViewField`](../resourceusageviewfield/).

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | يحوّل نسخة من الفئة `ResourceUsageViewFieldCollection` إلى قائمة تحتوي على نسخ الفئة [`ResourceUsageViewField`](../resourceusageviewfield/). |

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

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


