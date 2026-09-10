---
title: "RiskPattern"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 60
url: /ja/python-net/aspose.tasks.riskanalysis/riskpattern/
---

## RiskPattern class

プロジェクトタスクのリスクパターンを表します。

RiskPattern 型は次のメンバーを公開します：
## コンストラクタ
| 名前 | 説明 |
| :- | :- |
| RiskPattern(task) | 新しい [RiskPattern](/tasks/python-net/aspose.tasks.riskanalysis/riskpattern/) クラスのインスタンスを初期化します。 |
## プロパティ
| 名前 | 説明 |
| :- | :- |
| task | このリスクパターンが適用されるプロジェクト タスクを取得します。 |
| distribution | Monte Carlo シミュレーションで使用される確率分布を取得または設定します。<br/>            デフォルト値は ProbabilityDistributionType.Normal です。 |
| confidence_level | 実際に生成された値が楽観的および悲観的な見積もりの範囲内に収まる時間の割合に対応する信頼水準を取得または設定します。<br/>            デフォルト値は CL99 です。 |
| optimistic | ベストシナリオのプロジェクトで起こり得る最も可能性の高いタスク期間のパーセンテージを取得または設定します。<br/>            デフォルト値は 75 で、これは推定されたタスク期間が 4 日の場合、楽観的な期間は 3 日になることを意味します。 |
| pessimistic | 最悪シナリオのプロジェクトで起こり得る最も可能性の高いタスク期間のパーセンテージを取得または設定します。<br/>            デフォルト値は 125 で、これは推定されたタスク期間が 4 日の場合、悲観的な期間は 5 日になることを意味します。 |

### 関連項目

* namespace [aspose.tasks.riskanalysis](/tasks/python-net/aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](/tasks/python-net/)

