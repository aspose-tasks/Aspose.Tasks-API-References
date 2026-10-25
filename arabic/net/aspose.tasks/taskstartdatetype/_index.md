---
title: "تعداد TaskStartDateType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.TaskStartDateType. يحدد نوع تاريخ بدء المهمة"
type: docs
weight: 2450
url: /ar/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

يحدد نوع تاريخ بدء المهمة.

```csharp
public enum TaskStartDateType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | لم يتم تعريف قيمة الحقل في ملف المشروع الأصلي. |
| ProjectStartDate | `0` | تاريخ بدء المشروع |
| CurrentDate | `1` | التاريخ الحالي |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يوضح كيفية تعيين تاريخ البدء الافتراضي للمهمة كـ 'CurrentDate'.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


