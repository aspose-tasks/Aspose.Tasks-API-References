---
title: "ReportType"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトのグラフィカルレポートのタイプ。"
type: docs
weight: 247
url: /ja/java/com.aspose.tasks/reporttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ReportType extends System.Enum
```

プロジェクトのグラフィカルレポートのタイプです。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [BestPracticeAnalyzer](#BestPracticeAnalyzer) | 実作業がないタスク、未割り当てタスク、期間が8時間未満のタスク、およびリソースに割り当てられたサマリーを表示します。 |
| [Burndown](#Burndown) | 作業バーンダウンとタスクバーンダウンのチャートを含みます。 |
| [CashFlow](#CashFlow) | すべてのトップレベルタスクの四半期ごとのコストと累積コストを表示します。 |
| [CostOverruns](#CostOverruns) | タスクとリソース別のコスト差異を表示します。 |
| [CostOverview](#CostOverview) | プロジェクトの開始日と終了日、現在の予定コストと残りコスト、完了率%およびトップレベルタスクのコスト値を表示します。 |
| [CriticalTasks](#CriticalTasks) | クリティカルなプロジェクトタスクを表示します。 |
| [LateTasks](#LateTasks) | 遅延しているプロジェクトタスクを表示します。 |
| [Milestones](#Milestones) | 遅延している、進行中の、完了したマイルストーンを表示します。 |
| [OverallocatedResources](#OverallocatedResources) | 過剰割り当てリソースの残り作業時間数を表示します。 |
| [ProjectOverview](#ProjectOverview) | プロジェクトの開始日と終了日、完了した期間の割合、トップレベルタスクの完了率、そして今後のマイルストーンを表示します。 |
| [ResourceCostOverview](#ResourceCostOverview) | リソースごとのベースライン、実績、残りのコストを表示します。 |
| [ResourceOverview](#ResourceOverview) | リソースごとのベースライン、実績、残りの作業を表示します。 |
| [SlippingTasks](#SlippingTasks) | ベースラインの終了日を過ぎて完了予定のタスクを表示します（ベースラインは setInternal で設定する必要があります）。 |
| [TaskCostOverview](#TaskCostOverview) | すべてのトップレベルタスクのベースライン、実績、残りのコストを表示します。 |
| [UpcomingTask](#UpcomingTask) | 現在週に期限があるタスクと、現在週に開始するタスクを表示します。 |
| [WorkOverview](#WorkOverview) | 各トップレベルタスクのベースライン、実績、残りの作業と、作業リソースの作業量を表示します。 |
### BestPracticeAnalyzer {#BestPracticeAnalyzer}
```
public static final int BestPracticeAnalyzer
```


実作業がないタスク、未割り当てタスク、期間が8時間未満のタスク、およびリソースに割り当てられたサマリーを表示します。

### Burndown {#Burndown}
```
public static final int Burndown
```


作業バーンダウンチャートとタスクバーンダウンチャートを含みます。作業バーンダウンチャートは、メンバーが完了した作業量、プロジェクト終了日までに完了予定の作業量、そしてこの時点で完了すると見込まれる作業量のベースライン推定を示します。タスクバーンダウンチャートは、完了したタスク数、残りのタスク数、そしてこの時点で完了すると見込まれるタスク数のベースライン推定を示します。

### CashFlow {#CashFlow}
```
public static final int CashFlow
```


すべてのトップレベルタスクの四半期ごとのコストと累積コストを表示します。

### CostOverruns {#CostOverruns}
```
public static final int CostOverruns
```


タスクとリソース別のコスト差異を表示します。

### CostOverview {#CostOverview}
```
public static final int CostOverview
```


プロジェクトの開始日と終了日、現在の予定コストと残りコスト、完了率%およびトップレベルタスクのコスト値を表示します。

### CriticalTasks {#CriticalTasks}
```
public static final int CriticalTasks
```


クリティカルなプロジェクトタスクを表示します。

### LateTasks {#LateTasks}
```
public static final int LateTasks
```


遅延しているプロジェクトタスクを表示します。

### Milestones {#Milestones}
```
public static final int Milestones
```


遅延している、進行中の、完了したマイルストーンを表示します。

### OverallocatedResources {#OverallocatedResources}
```
public static final int OverallocatedResources
```


過剰割り当てリソースの残り作業時間数を表示します。

### ProjectOverview {#ProjectOverview}
```
public static final int ProjectOverview
```


プロジェクトの開始日と終了日、完了した期間の割合、トップレベルタスクの完了率、そして今後のマイルストーンを表示します。

### ResourceCostOverview {#ResourceCostOverview}
```
public static final int ResourceCostOverview
```


リソースごとのベースライン、実績、残りのコストを表示します。

### ResourceOverview {#ResourceOverview}
```
public static final int ResourceOverview
```


リソースごとのベースライン、実績、残りの作業を表示します。

### SlippingTasks {#SlippingTasks}
```
public static final int SlippingTasks
```


ベースラインの終了日を過ぎて完了予定のタスクを表示します（ベースラインは setInternal で設定する必要があります）。

### TaskCostOverview {#TaskCostOverview}
```
public static final int TaskCostOverview
```


すべてのトップレベルタスクのベースライン、実績、残りのコストを表示します。

### UpcomingTask {#UpcomingTask}
```
public static final int UpcomingTask
```


現在週に期限があるタスクと、現在週に開始するタスクを表示します。

### WorkOverview {#WorkOverview}
```
public static final int WorkOverview
```


各トップレベルタスクのベースライン、実績、残りの作業と、作業リソースの作業量を表示します。

