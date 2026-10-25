---
title: "ExtendedAttributeDefinition.SummaryRowsCalculationType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttributeDefinition. تحصل أو تعين نوع حساب قيمة السمات المخصصة لصفوف الملخص"
type: docs
weight: 260
url: /ar/net/aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/
---
## ExtendedAttributeDefinition.SummaryRowsCalculationType property

يحصل أو يضبط نوع حساب قيمة الخاصية المخصصة للصفوف الملخصة.

```csharp
public SummaryRowsCalculationType SummaryRowsCalculationType { get; set; }
```

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

* enum [SummaryRowsCalculationType](../../summaryrowscalculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


