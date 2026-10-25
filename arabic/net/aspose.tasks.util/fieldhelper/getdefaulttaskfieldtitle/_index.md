---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة FieldHelper. تُرجع عنوانًا افتراضيًا للحقل المحدد للمهمة"
type: docs
weight: 20
url: /ar/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

تُعيد عنوانًا افتراضيًا لحقل المهمة المحدد.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| taskKey | TaskKey | حقل المهمة للحصول على عنوان افتراضي. |

### قيمة الإرجاع

عنوان افتراضي للحقل المحدد للمهمة إذا كان يمكن عرض الحقل في عرض MS Project، وإلا يكون null.

## الأمثلة

يوضح كيفية الحصول على عنوان الحقل الافتراضي لحقل المهمة المحدد.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### انظر أيضًا

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


