---
title: "RiskAnalysisSettings"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "リスク分析を実行するための設定を指定します。"
type: docs
weight: 263
url: /ja/java/com.aspose.tasks/riskanalysissettings/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisSettings
```

リスク分析を実行するための設定を指定します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [RiskAnalysisSettings()](#RiskAnalysisSettings--) | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getIterationsCount()](#getIterationsCount--) | モンテカルロシミュレーションで使用する反復回数を取得します。 |
| [getPatterns()](#getPatterns--) | [RiskPattern](../../com.aspose.tasks/riskpattern) クラスのインスタンスを含むコレクションを取得します。 |
| [setIterationsCount(int value)](#setIterationsCount-int-) | モンテカルロシミュレーションで使用する反復回数を設定します。 |
### RiskAnalysisSettings() {#RiskAnalysisSettings--}
```
public RiskAnalysisSettings()
```


[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) クラスの新しいインスタンスを初期化します。

### getIterationsCount() {#getIterationsCount--}
```
public final int getIterationsCount()
```


モンテカルロシミュレーションで使用する反復回数を取得します。デフォルト値は 100 です。

**Returns:**
int - モンテカルロシミュレーションで使用する反復回数。
### getPatterns() {#getPatterns--}
```
public final RiskPatternCollection getPatterns()
```


[RiskPattern](../../com.aspose.tasks/riskpattern) クラスのインスタンスを含むコレクションを取得します。

**Returns:**
[RiskPatternCollection](../../com.aspose.tasks/riskpatterncollection) - a collection containing the instances of the [RiskPattern](../../com.aspose.tasks/riskpattern) class.
### setIterationsCount(int value) {#setIterationsCount-int-}
```
public final void setIterationsCount(int value)
```


モンテカルロシミュレーションで使用する反復回数を設定します。デフォルト値は 100 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | モンテカルロシミュレーションで使用する反復回数。 |

