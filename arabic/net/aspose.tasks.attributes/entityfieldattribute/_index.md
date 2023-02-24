---
title: Class EntityFieldAttribute
second_title: Aspose.Tasks لمرجع .NET API
description: Aspose.Tasks.Attributes.EntityFieldAttribute فصل. يمثل سمة لخصائص الكيان .
type: docs
weight: 70
url: /ar/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

يمثل سمة لخصائص الكيان .

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Default_Constructor |

### ملاحظات

السمة المستخدمة لـ[`Task`](../../aspose.tasks/task/) و[`Resource`](../../aspose.tasks/resource/) و[`Project`](../../aspose.tasks/project/) و[`ResourceAssignment`](../../aspose.tasks/resourceassignment/) خصائص الكيان فقط ، ويبسط تعدادها.

### أمثلة

كيفية تعداد الخصائص باستخدام **EntityField** السمة:

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

### أنظر أيضا

* مساحة الاسم [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* المجسم [Aspose.Tasks](../../)


