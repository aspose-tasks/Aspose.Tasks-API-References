---
title: "الفئة GraphicalIndicatorCriteria"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.GraphicalIndicatorCriteria. تمثل معيار مؤشر رسومي واحد مرتبط بصفة موسعة"
type: docs
weight: 730
url: /ar/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

يمثل معيار مؤشر رسومي واحد مرتبط بصفة موسعة.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | ينشئ مثيلاً جديداً من النوع `GraphicalIndicatorCriteria`. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | ينشئ مثيلاً جديداً من النوع `GraphicalIndicatorCriteria`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | يحصل على فهرس الصورة التي سيتم عرضها عندما يفي الحقل بالمعايير. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | يحصل على قيمة تعداد [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) الذي يحدد الصفوف التي يُطبق عليها المؤشر. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | يحصل على نوع المقارنة التي تُجرى بين قيمة الصفة الموسعة والقيم التي تعمل كمعيار لتطبيق المؤشر الرسومي. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | يحصل على القيمة المستخدمة لاختبار قيمة السمة الموسعة. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | يحصل على القيمة الثانية المستخدمة لاختبار قيمة السمة الموسعة في حالة أنواع المقارنة 'IsWithin' و 'IsNotWithin'. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | يرجع تمثيلًا نصيًا لنسخة الفئة `GraphicalIndicatorCriteria`. |

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


