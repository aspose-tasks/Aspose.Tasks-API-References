---
title: "Enum RollupType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.RollupType enum. يحدد نوع التجميع"
type: docs
weight: 1950
url: /ar/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

يحدد نوع التجميع.

```csharp
public enum RollupType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Null | `0` | يشير إلى نوع التجميع Null. |
| Maximum | `1` | يشير إلى نوع التجميع Maximum. |
| Minimum | `2` | يشير إلى نوع التجميع Minimum. |
| Count | `3` | يشير إلى نوع التجميع Count. |
| Sum | `4` | يشير إلى نوع التجميع Sum. |
| Average | `5` | يشير إلى نوع التجميع Average. |
| AverageFirstSublevel | `6` | يشير إلى نوع التجميع Average First Sublevel. |
| CountFirstSublevel | `7` | يشير إلى نوع التجميع Count First Sublevel. |
| CountNonsummaries | `8` | يشير إلى نوع التجميع Count Non-Summaries. |

## الأمثلة

يوضح كيفية العمل مع نوع الحساب لتعريف سمة موسعة.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// إنشاء تعريف سمة بنوع 'Formula' حيث يتم حساب القيم للمهام الفرعية والمهام الملخصة باستخدام الصيغة.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// إنشاء تعريف سمة حيث يتم حساب القيم للمهام الملخصة باستخدام نوع التجميع 'Average'.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


