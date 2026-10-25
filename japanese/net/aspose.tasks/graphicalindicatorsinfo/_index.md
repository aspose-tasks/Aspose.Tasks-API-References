---
title: "クラス GraphicalIndicatorsInfo"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.GraphicalIndicatorsInfo クラス。拡張属性に関連付けられたグラフィカルインジケータ定義を表します。"
type: docs
weight: 760
url: /ja/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

拡張属性に関連付けられたグラフィカルインジケータ定義を表します。

```csharp
public sealed class GraphicalIndicatorsInfo
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | `GraphicalIndicatorsInfo` 型の新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | グラフィカルインジケータ基準のリストを取得します。 |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | プロジェクトサマリ行がサマリ行から基準を継承するかどうかを示すフラグを取得または設定します。 |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | フィールドのデータ値をツールチップに表示するかどうかを示すフラグを取得または設定します。 |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | サマリ行が非サマリ行から基準を継承するかどうかを示すフラグを取得または設定します。 |

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


