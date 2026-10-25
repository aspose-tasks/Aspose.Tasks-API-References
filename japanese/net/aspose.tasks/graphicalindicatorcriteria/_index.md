---
title: "クラス GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.GraphicalIndicatorCriteria クラス。拡張属性に関連付けられた 1 つのグラフィカルインジケータ基準を表します"
type: docs
weight: 730
url: /ja/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

拡張属性に関連付けられた 1 つのグラフィカルインジケータ基準を表します。

```csharp
public sealed class GraphicalIndicatorCriteria
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | `GraphicalIndicatorCriteria` 型の新しいインスタンスを初期化します。 |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | `GraphicalIndicatorCriteria` 型の新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | フィールドが基準を満たしたときに表示する画像のインデックスを取得します。 |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) 列挙体の値を取得します。この列挙体はインジケータが適用される行を示します。 |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | 拡張属性の値と、グラフィカルインジケータの適用基準として機能する値との比較タイプを取得します。[`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | 拡張属性の値をテストするために使用される値を取得します。 |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | 'IsWithin' および 'IsNotWithin' の比較タイプの場合に、拡張属性の値をテストするために使用される第2の値を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | `GraphicalIndicatorCriteria` クラスのインスタンスの文字列表現を返します。 |

## 例

グラフィカルインジケータ情報の取得方法を示します。

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


