---
title: "PrimaveraProjectProperties"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Primavera の XER または P6XML ファイルから読み込まれたプロジェクトの Primavera 固有プロパティを表します。"
type: docs
weight: 205
url: /ja/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Primavera ファイル（XER または P6XML）から読み取られたプロジェクトの Primavera 固有プロパティを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | 現在のプロジェクトのベースラインプロジェクトの配列を取得します。 |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | 重要なアクティビティを定義する方法（最長経路または総フロートアプローチ）を取得します。 |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | 総フロート法が使用される場合に重要なアクティビティを定義するために使用される閾値を取得します。 |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | 現在のベースラインプロジェクトの Id を取得します。 |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | プロジェクト間のアクティビティ関係を無視するかどうかを定義するフラグを取得します。 |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | プロジェクトのスケジューリング時にアクティビティを重要としてマークすべきかどうかを定義するフラグを取得します。 |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Primavera プロジェクトで関係遅延をスケジュールする際に使用するカレンダーを定義するオプションを取得します。 |
| [getShortName()](#getShortName--) | プロジェクトの短縮名（プロジェクト ID）を取得します。 |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | アクティビティの完了日を期待完了日としてスケジュールすべきかどうかを定義するフラグを取得します。 |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


現在のプロジェクトのベースラインプロジェクトの配列を取得します。エクスポートされたベースラインを含む Primavera XML ファイルから読み込まれたプロジェクトに適用可能です。

**Returns:**
com.aspose.tasks.Project[] - 現在のプロジェクトのベースラインプロジェクトの配列。
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


重要なアクティビティを定義する方法（最長経路または総フロートアプローチ）を取得します。

**Returns:**
int - 重要なアクティビティを定義する方法（最長経路または総フロートアプローチ）。
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


総フロート法が使用される場合に重要なアクティビティを定義するために使用される閾値を取得します。

**Returns:**
java.lang.Double - 総フロート法が使用される場合に重要なアクティビティを定義するために使用される閾値。
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


現在のベースラインプロジェクトの Id を取得します。エクスポートされたベースラインを含む Primavera XML ファイルから読み込まれたプロジェクトに適用可能です。

**Returns:**
int - 現在のベースラインプロジェクトの Id。
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


プロジェクト間のアクティビティ関係を無視するかどうかを定義するフラグを取得します。

**Returns:**
boolean - プロジェクト間のアクティビティ関係を無視するかどうかを定義するフラグ。
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


プロジェクトのスケジューリング時にアクティビティを重要としてマークすべきかどうかを定義するフラグを取得します。

**Returns:**
boolean - プロジェクトのスケジューリング時にアクティビティを重要としてマークすべきかどうかを定義するフラグ。
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Primavera プロジェクトで関係遅延をスケジュールする際に使用するカレンダーを定義するオプションを取得します。

**Returns:**
int - Primavera プロジェクトで関係遅延をスケジュールする際に使用するカレンダーを定義するオプション。
### getShortName() {#getShortName--}
```
public final String getShortName()
```


プロジェクトの短縮名（プロジェクト ID）を取得します。

**Returns:**
java.lang.String - プロジェクトの短縮名（プロジェクト ID）。
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


アクティビティの完了日を期待完了日としてスケジュールすべきかどうかを定義するフラグを取得します。

**Returns:**
boolean - アクティビティの完了日を期待完了日としてスケジュールすべきかどうかを定義するフラグ。
