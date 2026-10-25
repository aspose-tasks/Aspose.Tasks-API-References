---
title: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "拡張属性に関連付けられたグラフィカル インジケータ基準のひとつを表します。"
type: docs
weight: 115
url: /ja/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

拡張属性に関連付けられたグラフィカル インジケータ基準のひとつを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | 新しい [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 型のインスタンスを初期化します。 |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | 新しい [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 型のインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | フィールドが条件を満たしたときに表示する画像のインデックスを取得します。 |
| [getRowType()](#getRowType--) | インジケーターが適用される行を示す [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 列挙体の値を取得します。 |
| [getTest()](#getTest--) | 拡張属性の値と、グラフィカルインジケーターの適用基準となる値との比較タイプを取得します。 |
| [getValue1()](#getValue1--) | 拡張属性の値をテストするために使用される値を取得します。 |
| [getValue2()](#getValue2--) | 「IsWithin」および「IsNotWithin」比較タイプの場合に、拡張属性の値をテストするために使用される第2の値を取得します。 |
| [toString()](#toString--) | [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) クラスのインスタンスの文字列表現を返します。 |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


新しい [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 型のインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| rowType | int | インジケーターが適用される行を示す [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 列挙体の値 |
| test | int | 基準が実行する比較のタイプを示す [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) の値。 |
| imageIndex | int | フィールドが条件を満たしたときに表示する画像のインデックス |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 条件チェックで使用される値。 |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 「IsWithin」および「IsNotWithing」条件の場合に、条件チェックで使用される第2の値（区間の終端）。 |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


新しい [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 型のインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| rowType | int | インジケーターが適用される行を示す [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 列挙体の値 |
| test | int | 基準が実行する比較のタイプを示す [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) の値。 |
| imageIndex | int | フィールドが条件を満たしたときに表示する画像のインデックス |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 条件チェックで使用される値。 |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


フィールドが条件を満たしたときに表示する画像のインデックスを取得します。

**Returns:**
int - フィールドが条件を満たしたときに表示する画像のインデックス。
### getRowType() {#getRowType--}
```
public final int getRowType()
```


インジケーターが適用される行を示す [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 列挙体の値を取得します。

**Returns:**
int - インジケーターが適用される行を示す [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 列挙体の値。
### getTest() {#getTest--}
```
public final int getTest()
```


拡張属性の値と、グラフィカルインジケーターの適用基準となる値との比較タイプを取得します。 [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - 拡張属性の値と、グラフィカルインジケーターの適用基準となる値との比較タイプ。
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


拡張属性の値をテストするために使用される値を取得します。

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


「IsWithin」および「IsNotWithin」比較タイプの場合に、拡張属性の値をテストするために使用される第2の値を取得します。

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


[GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) クラスのインスタンスの文字列表現を返します。

**Returns:**
java.lang.String - このオブジェクトの文字列表現。
