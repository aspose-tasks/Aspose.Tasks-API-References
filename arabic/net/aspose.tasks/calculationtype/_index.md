---
title: "التعداد CalculationType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.CalculationType. يحدد نوع حساب قيمة السمات المخصصة"
type: docs
weight: 220
url: /ar/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

يحدد نوع حساب قيمة السمة المخصصة.

```csharp
public enum CalculationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يعني أن السمة الموسعة لا تحتوي على جدول بحث للمعادلة وتخزن ببساطة القيمة التي يحددها المستخدم. |
| Lookup | `1` | يعني أن قيمة السمة الموسعة مقيدة بالقيم الموجودة في جدول البحث. |
| Formula | `2` | يعني أن قيمة السمة الموسعة تُحسب باستخدام المعادلة المعرفة في [`Formula`](../extendedattributedefinition/formula/). |

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


