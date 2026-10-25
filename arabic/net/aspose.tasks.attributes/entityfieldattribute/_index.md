---
title: "فئة EntityFieldAttribute"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Attributes.EntityFieldAttribute. تمثل سمة لخصائص الكيان."
type: docs
weight: 70
url: /ar/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

يمثل سمة لخصائص الكيان.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | المنشئ الافتراضي. |

## ملاحظات

السمة المستخدمة لـ [`Task`](../../aspose.tasks/task/)، [`Resource`](../../aspose.tasks/resource/)، [`Project`](../../aspose.tasks/project/) و[`ResourceAssignment`](../../aspose.tasks/resourceassignment/) خصائص الكيان فقط، وتبسط تعدادها.

## الأمثلة

كيفية تعداد الخصائص باستخدام السمة **EntityField**:

```csharp
[C#]
var project = new Project("sample.mpp");
foreach (var task in project.SelectAllChildTasks())
{
    Console.WriteLine("Task:");
    foreach (var propInfo in typeof(Task).GetProperties().Where(propInfo => propInfo.GetCustomAttribute{Attributes.EntityFieldAttribute}() != null))
    {
        Console.WriteLine(string.Format("{0}: {1}", propInfo.Name, propInfo.GetValue(task)));
    }
}
```

### انظر أيضًا

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


