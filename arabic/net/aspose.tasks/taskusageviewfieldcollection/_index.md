---
title: "الفئة TaskUsageViewFieldCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TaskUsageViewFieldCollection. تمثل مجموعة من قيم TaskUsageViewField"
type: docs
weight: 2500
url: /ar/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

تمثل مجموعة من قيم [`TaskUsageViewField`](../taskusageviewfield/).

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | يرجع قائمة تحتوي على جميع العناصر من هذه المجموعة. |

## الأمثلة

يوضح كيفية التعامل مع مجموعة الحقول لنسخة TaskUsageView.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// يمكن تحويل المجموعة إلى قائمة من TaskUsageViewField.
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### انظر أيضًا

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


