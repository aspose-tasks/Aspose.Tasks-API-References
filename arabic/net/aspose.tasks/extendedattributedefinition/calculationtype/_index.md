---
title: "ExtendedAttributeDefinition.CalculationType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttributeDefinition. يحصل أو يضبط نوع الحساب لقيمة السمة المخصصة"
type: docs
weight: 80
url: /ar/net/aspose.tasks/extendedattributedefinition/calculationtype/
---
## ExtendedAttributeDefinition.CalculationType property

يحصل أو يعيّن نوع حساب قيمة السمة المخصصة.

```csharp
public CalculationType CalculationType { get; set; }
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

* enum [CalculationType](../../calculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


