---
title: "الفئة GraphicalIndicatorsInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.GraphicalIndicatorsInfo. تمثل تعريف مؤشرات رسومية مرتبط بصفة موسعة"
type: docs
weight: 760
url: /ar/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

يمثل تعريفًا للمؤشرات الرسومية مرتبطًا بصفة موسعة.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | ينشئ مثيلًا جديدًا من النوع `GraphicalIndicatorsInfo`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | يحصل على قائمة بمعايير المؤشر الرسومية. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | يحصل أو يضبط العلامة التي تشير إلى ما إذا كان صف ملخص المشروع يرث المعايير من صفوف الملخص. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | يحصل أو يضبط العلامة التي تشير إلى ما إذا كان يجب عرض قيم البيانات للحقل في تلميحات الأدوات. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | يحصل أو يضبط العلامة التي تشير إلى ما إذا كانت صفوف الملخص ترث المعايير من صفوف غير الملخص. |

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


