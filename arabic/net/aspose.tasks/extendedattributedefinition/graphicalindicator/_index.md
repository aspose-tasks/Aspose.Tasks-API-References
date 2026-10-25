---
title: "ExtendedAttributeDefinition.GraphicalIndicator"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttributeDefinition. تحصل أو تعيين معلومات مؤشرات رسومية مرتبطة بالسمة الموسعة. قابلة للتطبيق على تنسيق MPP."
type: docs
weight: 160
url: /ar/net/aspose.tasks/extendedattributedefinition/graphicalindicator/
---
## ExtendedAttributeDefinition.GraphicalIndicator property

يحصل أو يضبط معلومات مؤشرات رسومية مرتبطة بالخاصية الموسعة. ينطبق على تنسيق MPP.

```csharp
public GraphicalIndicatorsInfo GraphicalIndicator { get; set; }
```

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

* class [GraphicalIndicatorsInfo](../../graphicalindicatorsinfo/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


