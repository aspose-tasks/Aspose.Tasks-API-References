---
title: "TaskUsageView.FieldCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskUsageView. يحصل على كائن TaskUsageViewFieldCollection لهذا TaskUsageView"
type: docs
weight: 10
url: /ar/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

يحصل على كائن [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) لهذا TaskUsageView.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## الأمثلة

يعرض كيفية قراءة حقول عرض استخدام المهمة.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### انظر أيضًا

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)


