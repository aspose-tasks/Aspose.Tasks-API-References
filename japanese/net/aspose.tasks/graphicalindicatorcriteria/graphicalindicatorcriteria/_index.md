---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "GraphicalIndicatorCriteria コンストラクタ。GraphicalIndicatorCriteria 型の新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

[`GraphicalIndicatorCriteria`](../) 型の新しいインスタンスを初期化します。

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) 列挙体の値で、インジケーターが適用される行を示します。 |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) の値で、基準が実行する比較の種類を示します。 |
| imageIndex | Int32 | フィールドが基準を満たしたときに表示する画像のインデックスです。 |
| value1 | GraphicalIndicatorCriteriaValue | 条件チェックで使用される値です。 |
| value2 | GraphicalIndicatorCriteriaValue | 「IsWithin」および「IsNotWithing」条件の場合に条件チェックで使用される第2の値（区間の終端）です。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | コンストラクタに不正な引数の組み合わせが渡されたときにスローされます。 |

### 関連項目

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

[`GraphicalIndicatorCriteria`](../) 型の新しいインスタンスを初期化します。

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) 列挙体の値で、インジケーターが適用される行を示します。 |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) の値で、基準が実行する比較の種類を示します。 |
| imageIndex | Int32 | フィールドが基準を満たしたときに表示する画像のインデックスです。 |
| 値 | GraphicalIndicatorCriteriaValue | 条件チェックで使用される値です。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | コンストラクタに不正な引数の組み合わせが渡されたときにスローされます。 |
| ArgumentException | IsWithin または IsNotWithing の値がテスト引数に渡されたときです。 |

### 関連項目

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


