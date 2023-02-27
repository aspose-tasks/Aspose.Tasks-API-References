---
title: Enum ConstraintType
second_title: Aspose.Tasks لمرجع .NET API
description: Aspose.Tasks.ConstraintType تعداد. تحديد القيد على تاريخ البدء أو الانتهاء لمهمة.
type: docs
weight: 330
url: /ar/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

تحديد القيد على تاريخ البدء أو الانتهاء لمهمة.

```csharp
public enum ConstraintType
```

### قيم

| اسم | قيمة | وصف |
| --- | --- | --- |
| Undefined | `-1` | لم يتم تحديد القيمة في ملف المشروع الأصلي. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) و[`Finish`](../tsk/finish/) مواعيد[`Task`](../task/) تمت جدولة ASAP فيما يتعلق بالوالد[`Start`](../tsk/start/) و[`Finish`](../tsk/finish/)التواريخ والنظر[`TaskLinks`](../project/tasklinks/) . |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) و[`Finish`](../tsk/finish/) مواعيد[`Task`](../task/) من المقرر ALAP فيما يتعلق بالوالد[`Start`](../tsk/start/) و[`Finish`](../tsk/finish/)التواريخ والنظر[`TaskLinks`](../project/tasklinks/) . |
| MustStartOn | `2` | يجب البدء في |
| MustFinishOn | `3` | يجب الانتهاء في |
| StartNoEarlierThan | `4` | لم تبدأ قبل |
| StartNoLaterThan | `5` | لا تبدأ بعد |
| FinishNoEarlierThan | `6` | لم يتم الانتهاء في وقت سابق من |
| FinishNoLaterThan | `7` | لا ينتهي بعد |

### ملاحظات

أثناء التصدير إلى XML ، سيتم حذف القيم غير المعرفة من XML الناتج.

### أنظر أيضا

* مساحة الاسم [Aspose.Tasks](../../aspose.tasks/)
* المجسم [Aspose.Tasks](../../)


