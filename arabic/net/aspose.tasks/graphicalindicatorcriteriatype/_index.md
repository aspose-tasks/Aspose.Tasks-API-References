---
title: "التعداد GraphicalIndicatorCriteriaType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.GraphicalIndicatorCriteriaType. يمثل موضع معايير المؤشر الرسومي."
type: docs
weight: 740
url: /ar/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

يمثل موضع معايير المؤشر الرسومي.

```csharp
public enum GraphicalIndicatorCriteriaType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| NonSummaryRows | `0` | يمثل الصفوف غير الملخصة. |
| SummaryRows | `1` | يمثل صفوف الملخص. |
| ProjectSummary | `2` | يمثل صف مهمة ملخص المشروع. |

## الأمثلة

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


