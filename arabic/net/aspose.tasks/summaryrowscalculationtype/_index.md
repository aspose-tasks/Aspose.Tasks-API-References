---
title: "تعداد SummaryRowsCalculationType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.SummaryRowsCalculationType. يحدد نوع حساب قيمة السمات المخصصة للصفوف الملخصة"
type: docs
weight: 2310
url: /ar/net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

يحدد نوع حساب قيمة السمة المخصصة لصفوف الملخص.

```csharp
public enum SummaryRowsCalculationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يعني أن قيمة السمة المخصصة للصفوف الملخصة غير محسوبة. |
| Rollup | `1` | يعني أن قيمة السمة المخصصة للصفوف الملخصة تُحسب باستخدام دالة التجميع المحددة في [`RollupType`](../extendedattributedefinition/rolluptype/). |
| UseFormula | `2` | يعني أن قيمة السمة المخصصة للصفوف الملخصة تُحسب باستخدام الصيغة المحددة في [`Formula`](../extendedattributedefinition/formula/). |

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


