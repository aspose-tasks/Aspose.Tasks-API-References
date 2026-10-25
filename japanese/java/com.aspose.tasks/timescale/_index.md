---
title: "Timescale"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトがグラフィック形式にエクスポートされる際に、ガントチャートのタスク使用状況またはリソース使用状況ビューでタイムスケールを描画する方法を指定するオプションを定義します。"
type: docs
weight: 323
url: /ja/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

プロジェクトをグラフィック形式でエクスポートする際に、ガントチャート、タスク使用、リソース使用ビューでタイムスケールをどのようにレンダリングするかを指定するオプションを定義します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [Days](#Days) | 最小の詳細レベルが1日である、事前定義された2層タイムスケールです。 |
| [DefinedInView](#DefinedInView) | プロジェクトビューのプロパティで定義されたタイムスケール設定を使用します: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | 最小の詳細レベルが1か月である、事前定義された2層タイムスケールです。 |
| [ThirdsOfMonths](#ThirdsOfMonths) | 詳細レベルが1か月の3分の1である、事前定義された2層タイムスケールです。 |
### Days {#Days}
```
public static final int Days
```


最小の詳細レベルが1日である、事前定義された2層タイムスケールです。

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


プロジェクトビューのプロパティで定義されたタイムスケール設定を使用します: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). ビュー データを含む形式で有効です。例えば、MPP 形式から読み込まれるプロジェクトなどです。

--------------------

ビューにタイムスケール設定が設定されていない場合、代わりに事前定義された Timescale.Days 設定が使用されます。

### Months {#Months}
```
public static final int Months
```


最小の詳細レベルが1か月である、事前定義された2層タイムスケールです。

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


詳細レベルが1か月の3分の1である、事前定義された2層タイムスケールです。

