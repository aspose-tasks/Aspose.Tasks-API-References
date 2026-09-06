---
title: "الفئة GraphicalIndicatorCriteriaValue"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.GraphicalIndicatorCriteriaValue. تمثّل قيمة تُستخدم في فحص الشرط لمعايير المؤشرات الرسومية"
type: docs
weight: 750
url: /ar/net/aspose.tasks/graphicalindicatorcriteriavalue/
---
## GraphicalIndicatorCriteriaValue class

يمثل قيمة تُستخدم في فحص الشرط لمعايير المؤشرات الرسومية.

```csharp
public sealed class GraphicalIndicatorCriteriaValue
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_1)(bool) | ينشئ مثيلًا من الفئة GraphicalIndicatorCriteriaValue بقيمة علم ثابتة (bool). |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_2)(DateTime) | ينشئ مثيلًا من الفئة GraphicalIndicatorCriteriaValue بقيمة DateTime ثابتة. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_3)(decimal) | ينشئ مثيلًا من الفئة GraphicalIndicatorCriteriaValue بقيمة عشرية ثابتة. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor)(Duration) | ينشئ مثيلًا من الفئة GraphicalIndicatorCriteriaValue بقيمة Duration ثابتة. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_4)(string) | ينشئ مثيلًا من الفئة GraphicalIndicatorCriteriaValue بقيمة سلسلة ثابتة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/isfieldlink/) { get; } | يحصل على ما إذا كان المثيل الحالي رابط حقل (يمثل قيمة حقل). |
| [RawValue](../../aspose.tasks/graphicalindicatorcriteriavalue/rawvalue/) { get; } | يحصل على الثابت الأساسي لقيمة الحقل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [CreateFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/createfieldlink/)(Field) | ينشئ مثيلاً من فئة GraphicalIndicatorCriteriaValue تمثل قيمة الحقل المحدد في MS Project. |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteriavalue/tostring/)() | يرجع سلسلة تمثل الكائن الحالي. |

## الأمثلة

يوضح كيفية استرجاع معلومات المؤشرات الرسومية.

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

يوضح كيفية إعداد مؤشر رسومي لسمة موسعة.

```csharp
Project project = new Project();

var def = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number field");
project.ExtendedAttributes.Add(def);
def.GraphicalIndicator = new GraphicalIndicatorsInfo();

GraphicalIndicatorCriteria criteria1 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsLessThan,
    2,
    new GraphicalIndicatorCriteriaValue(100m));

// معيار 'IsWithin' يتطلب قيمتين.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// معيار 'IsAnyValue' لا يتطلب قيمًا.
GraphicalIndicatorCriteria criteria3 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsAnyValue,
    4,
    null);

def.GraphicalIndicator.Criteria.Add(criteria1);
def.GraphicalIndicator.Criteria.Add(criteria2);
def.GraphicalIndicator.Criteria.Add(criteria3);

def.GraphicalIndicator.ProjectSummaryInheritFromNonSummaryRows = true;
def.GraphicalIndicator.SummaryRowsInheritFromNonSummaryRows = true;
def.GraphicalIndicator.ShowDataValuesInTooltip = false;

project.Save(OutDir + "CreateGraphicalIndicators_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


