---
title: "RiskItemStatistics"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "分析されたプロジェクトのタスクの統計データを格納する項目を表します。"
type: docs
weight: 265
url: /ja/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

分析されたプロジェクトのタスクの統計データを格納する項目を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | リスク項目の期待値を取得します。 |
| [getItemType()](#getItemType--) | [RiskItemType](../../com.aspose.tasks/riskitemtype) 列挙体のインスタンスを取得します。 |
| [getMaximum()](#getMaximum--) | モンテカルロシミュレーション中に生成された最大値を取得します。 |
| [getMinimum()](#getMinimum--) | モンテカルロシミュレーション中に生成された最小値を取得します。 |
| [getPercentile(int percent)](#getPercentile-int-) | 生成されたサンプルの指定されたパーセンテージが下回る値を取得します。 |
| [getStandardDeviation()](#getStandardDeviation--) | リスク項目の標準偏差を取得します。 |
| [toString()](#toString--) | リスク項目の短い文字列表現を返します。 |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


リスク項目の期待値を取得します。

**Returns:**
java.util.Date - リスク項目の期待値。
### getItemType() {#getItemType--}
```
public final int getItemType()
```


[RiskItemType](../../com.aspose.tasks/riskitemtype) 列挙体のインスタンスを取得します。

**Returns:**
int - [RiskItemType](../../com.aspose.tasks/riskitemtype) 列挙体のインスタンス。
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


モンテカルロシミュレーション中に生成された最大値を取得します。

**Returns:**
java.util.Date - モンテカルロシミュレーション中に生成された最大値。
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


モンテカルロシミュレーション中に生成された最小値を取得します。

**Returns:**
java.util.Date - モンテカルロシミュレーション中に生成された最小値。
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


生成されたサンプルの指定されたパーセンテージが下回る値を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パーセント | int | 0 から 100 の間の指定されたパーセント。 |

**Returns:**
java.util.Date - 生成されたサンプルの指定されたパーセンテージが下回る値。
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


リスク項目の標準偏差を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


リスク項目の短い文字列表現を返します。表現の正確な詳細は未定義で、変更される可能性があります。

**Returns:**
java.lang.String - RiskItem オブジェクトを表す短い文字列。
