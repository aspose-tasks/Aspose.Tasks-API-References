---
title: "列挙体 GraphicalIndicatorCriteriaType"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaType 列挙体。グラフィカルインジケータ基準の配置を表します。"
type: docs
weight: 740
url: /ja/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

グラフィカルインジケータ基準の配置を表します。

```csharp
public enum GraphicalIndicatorCriteriaType
```

### 値

| 名前 | 値 | 説明 |
| --- | --- | --- |
| NonSummaryRows | `0` | 非サマリ行を表します。 |
| SummaryRows | `1` | サマリ行を表します。 |
| ProjectSummary | `2` | プロジェクトサマリタスク行を表します。 |

## 例

拡張属性に対するグラフィカルインジケータの設定方法を示します。

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

// 'IsWithin' 基準には 2 つの値が必要です。
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// 'IsAnyValue' 基準には値は必要ありません。
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

### 関連項目

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


