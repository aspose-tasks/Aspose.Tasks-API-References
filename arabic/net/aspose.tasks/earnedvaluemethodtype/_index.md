---
title: "تعداد EarnedValueMethodType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.EarnedValueMethodType. يحدد الطريقة المستخدمة لحساب القيمة المكتسبة"
type: docs
weight: 480
url: /ar/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

يحدد الطريقة المستخدمة لحساب القيمة المكتسبة.

```csharp
public enum EarnedValueMethodType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | لم يتم تعريف الحقل في ملف المشروع الأصلي. |
| PercentComplete | `0` | النسبة المكتملة |
| PhysicalPercentComplete | `1` | النسبة الفيزيائية المكتملة |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يوضح كيفية تحديد الطريقة المستخدمة لحساب القيمة المكتسبة (EarnedValueMethodType.PercentComplete).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// تعيين نوع طريقة القيمة المكتسبة إلى 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// العمل مع المشروع...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


