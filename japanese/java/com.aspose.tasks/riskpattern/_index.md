---
title: "RiskPattern"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトタスクのリスクパターンを表します。"
type: docs
weight: 268
url: /ja/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

プロジェクトタスクのリスクパターンを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | [RiskPattern](../../com.aspose.tasks/riskpattern) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | 実際に生成された値が楽観的および悲観的な見積もりの範囲内にある時間の割合に対応する信頼レベルを取得します。 |
| [getDistribution()](#getDistribution--) | モンテカルロシミュレーションで使用される確率分布を取得します。 |
| [getOptimistic()](#getOptimistic--) | 最良のプロジェクトシナリオで発生し得る最も可能性の高いタスク期間の割合を取得します。 |
| [getPessimistic()](#getPessimistic--) | 最悪のプロジェクトシナリオで発生し得る最も可能性の高いタスク期間の割合を取得します。 |
| [getTask()](#getTask--) | このリスクパターンが適用されるプロジェクトタスクを取得します。 |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | 実際に生成された値が楽観的および悲観的な見積もりの範囲内にある時間の割合に対応する信頼レベルを設定します。 |
| [setDistribution(int value)](#setDistribution-int-) | モンテカルロシミュレーションで使用される確率分布を設定します。 |
| [setOptimistic(int value)](#setOptimistic-int-) | 最良のプロジェクトシナリオで発生し得る最も可能性の高いタスク期間の割合を設定します。 |
| [setPessimistic(int value)](#setPessimistic-int-) | 最悪のプロジェクトシナリオで発生し得る最も可能性の高いタスク期間の割合を設定します。 |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


[RiskPattern](../../com.aspose.tasks/riskpattern) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | モンテカルロシミュレーションでこのリスクが適用される対象のプロジェクトタスクを指定します。 |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


実際に生成された値が楽観的および悲観的な見積もりの範囲内にある時間の割合に対応する信頼レベルを取得します。デフォルト値は CL99 です。

--------------------

`ConfidenceLevel` の列挙型で定義された値のいずれかを使用できます（[getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)）。

**Returns:**
int - 実際に生成された値が楽観的および悲観的な見積もりの範囲内にある時間の割合に対応する信頼レベル。
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Monte Carlo シミュレーションで使用される確率分布を取得します。デフォルト値は ProbabilityDistributionType.Normal です。

--------------------

[ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) 列挙体で定義された値のいずれかになります。

**Returns:**
int - Monte Carlo シミュレーションで使用される確率分布。
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


最も可能性の高いタスク期間のパーセンテージ（ベストシナリオで発生し得る）を取得します。デフォルト値は 75 で、これは推定されたタスク期間が 4 日の場合、楽観的な期間は 3 日になることを意味します。

**Returns:**
int - ベストシナリオで発生し得る最も可能性の高いタスク期間のパーセンテージ。
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


最も可能性の高いタスク期間のパーセンテージ（最悪シナリオで発生し得る）を取得します。デフォルト値は 125 で、これは推定されたタスク期間が 4 日の場合、悲観的な期間は 5 日になることを意味します。

**Returns:**
int - 最悪シナリオで発生し得る最も可能性の高いタスク期間のパーセンテージ。
### getTask() {#getTask--}
```
public final Task getTask()
```


このリスクパターンが適用されるプロジェクトタスクを取得します。

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


実際に生成された値が楽観的および悲観的な見積もりの範囲内にある時間の割合に対応する信頼レベルを設定します。デフォルト値は CL99 です。

--------------------

`ConfidenceLevel` の列挙型で定義された値のいずれかを使用できます（[getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 実際に生成された値が楽観的および悲観的な見積もりの範囲内にある時間の割合に対応する信頼レベル。 |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Monte Carlo シミュレーションで使用される確率分布を設定します。デフォルト値は ProbabilityDistributionType.Normal です。

--------------------

[ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) 列挙体で定義された値のいずれかになります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Monte Carlo シミュレーションで使用される確率分布。 |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


ベストシナリオで発生し得る最も可能性の高いタスク期間のパーセンテージを設定します。デフォルト値は 75 で、これは推定されたタスク期間が 4 日の場合、楽観的な期間は 3 日になることを意味します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | ベストシナリオで発生し得る最も可能性の高いタスク期間のパーセンテージ。 |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


最悪シナリオで発生し得る最も可能性の高いタスク期間のパーセンテージを設定します。デフォルト値は 125 で、これは推定されたタスク期間が 4 日の場合、悲観的な期間は 5 日になることを意味します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 最悪シナリオで発生し得る最も可能性の高いタスク期間のパーセンテージ。 |

