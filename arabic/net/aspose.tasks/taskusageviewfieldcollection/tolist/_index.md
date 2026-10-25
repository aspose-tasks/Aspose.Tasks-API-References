---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskUsageViewFieldCollection. تُرجع قائمة تحتوي على جميع العناصر من هذه المجموعة"
type: docs
weight: 20
url: /ar/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

يرجع قائمة تحتوي على جميع العناصر من هذه المجموعة.

```csharp
public IList<TaskUsageViewField> ToList()
```

### قيمة الإرجاع

تُرجع قائمة تحتوي على جميع العناصر من هذه المجموعة.

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

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


