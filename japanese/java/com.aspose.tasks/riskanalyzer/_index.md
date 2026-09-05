---
title: "RiskAnalyzer"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "指定されたリスク分析設定に基づいてモンテカルロシミュレーションを実行します。"
type: docs
weight: 264
url: /ja/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

指定されたリスク分析設定に基づいてモンテカルロシミュレーションを実行します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | 指定されたプロジェクトのリスク分析を実行します。 |
| [getSettings()](#getSettings--) | リスク分析に必要な設定を定義する [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) クラスのインスタンスを取得します。 |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | リスク分析に必要な設定を定義する [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) クラスのインスタンスを設定します。 |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


[RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | 指定された [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) クラスのインスタンスです。 |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


指定されたプロジェクトのリスク分析を実行します。分析はモンテカルロシミュレーションに基づいており、結果は [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) クラスのインスタンスです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 分析対象となる [Project](../../com.aspose.tasks/project) クラスの指定されたインスタンス。 |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


リスク分析に必要な設定を定義する [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) クラスのインスタンスを取得します。

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


リスク分析に必要な設定を定義する [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) クラスのインスタンスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | リスク分析に必要な設定を定義する [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) クラスのインスタンス。 |

