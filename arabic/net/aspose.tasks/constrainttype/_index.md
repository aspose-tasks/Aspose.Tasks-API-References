---
title: "التعداد ConstraintType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.ConstraintType. يحدد القيد على تاريخ البدء أو الانتهاء لمهمة"
type: docs
weight: 330
url: /ar/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

يحدد القيد على تاريخ بدء أو انتهاء المهمة.

```csharp
public enum ConstraintType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | القيمة لم تُعرّف في ملف المشروع الأصلي. |
| AsSoonAsPossible | `0` | تواريخ [`Start`](../tsk/start/) و[`Finish`](../tsk/finish/) للمهمة [`Task`](../task/) يتم جدولتها بأسرع ما يمكن بالنسبة إلى تواريخ الأصل [`Start`](../tsk/start/) و[`Finish`](../tsk/finish/) مع الأخذ في الاعتبار [`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) و [`Finish`](../tsk/finish/) تواريخ [`Task`](../task/) مجدولة ALAP بالنسبة إلى الأصل [`Start`](../tsk/start/) و [`Finish`](../tsk/finish/) مع مراعاة [`TaskLinks`](../project/tasklinks/). |
| MustStartOn | `2` | يجب أن يبدأ في |
| MustFinishOn | `3` | يجب أن ينتهي في |
| StartNoEarlierThan | `4` | لا يبدأ قبل |
| StartNoLaterThan | `5` | لا يبدأ بعد |
| FinishNoEarlierThan | `6` | لا ينتهي قبل |
| FinishNoLaterThan | `7` | لا ينتهي بعد |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يعرض كيفية تعيين القيد &lt;see cref="Aspose.Tasks.ConstraintType" /&gt; ConstraintType.AsSoonAsPossible لمهمة.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// تعيين القيد As Soon As Possible للمهمة ذات المعرف 11
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


