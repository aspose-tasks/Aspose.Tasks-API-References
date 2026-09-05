---
title: "PrimaveraTaskProperties"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Primavera の XER または P6XML ファイルから読み取られたタスクの Primavera 固有プロパティを表します。"
type: docs
weight: 209
url: /ja/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Primavera ファイル（XER または P6XML）から読み取られたタスクの Primavera 固有プロパティを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getActivityId()](#getActivityId--) | Primavera が使用するタスクの一意の識別子であるアクティビティ ID フィールドを取得します。 |
| [getActivityType()](#getActivityType--) | 「Activity Type」フィールドの値を取得します。 |
| [getActualExpenseCost()](#getActualExpenseCost--) | 実際の経費コストの値を取得します。 |
| [getActualLaborCost()](#getActualLaborCost--) | 実際の労働コストの値を取得します。 |
| [getActualLaborUnits()](#getActualLaborUnits--) | 実際の労働単位の値を取得します。 |
| [getActualMaterialCost()](#getActualMaterialCost--) | 実際の材料コストの値を取得します。 |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | 実際の非労働単位の値を取得します。 |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | 実際の非労働コストの値を取得します。 |
| [getActualTotalCost()](#getActualTotalCost--) | 実際のコストの合計値を取得します。 |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | 予算（または計画）された経費コストの値を取得します。 |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | 予算（または計画）された労働コストの値を取得します。 |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | 予算（または計画）された材料コストの値を取得します。 |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | 予算（または計画）された非労働コストの値を取得します。 |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | 予算（または計画）されたコストの合計値を取得します。 |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | 期間の完了率の値を取得します。 |
| [getDurationType()](#getDurationType--) | アクティビティの「Duration Type」フィールドの値を取得します。 |
| [getPercentCompleteType()](#getPercentCompleteType--) | アクティビティの「% Complete Type」フィールドの値を取得します。 |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Physical Percent Complete の値を取得します。 |
| [getPlannedDuration()](#getPlannedDuration--) | 元のまたは計画された期間を取得します――タスクの計画開始日から計画終了日までの合計作業時間です。 |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | 主要制約の日付を取得します。 |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | 主要制約のタイプを取得します。 |
| [getRawActivityType()](#getRawActivityType--) | アクティビティの「Activity Type」フィールドの生テキスト表現（ソースファイル内の形式）を取得します。 |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | アクティビティの「% Complete Type」フィールドの生テキスト表現（ソースファイル内の形式）を取得します。 |
| [getRawDurationType()](#getRawDurationType--) | アクティビティの「Duration Type」フィールドの生テキスト表現（ソースファイル内の形式）を取得します。 |
| [getRawStatus()](#getRawStatus--) | アクティビティの「Status」フィールドの生テキスト表現（ソースファイル内の形式）を取得します。 |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | 残りの早期完了日を取得します――アクティビティの残作業が完了するように予定されている日付です。 |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | 残りの早期開始日を取得します――アクティビティの残作業が開始されるように予定されている日付です。 |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | 残りの経費コストの値を取得します。 |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | 残りの労働単位の値を取得します。 |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | 残りの遅延完了日を取得します。 |
| [getRemainingLateStart()](#getRemainingLateStart--) | 残りの遅延開始日を取得します。 |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | 残りの非労働単位の値を取得します。 |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | 二次制約の日付を取得します。 |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | 二次制約のタイプを取得します。 |
| [getSequenceNumber()](#getSequenceNumber--) | WBS項目（サマリタスク）のシーケンス番号を取得します。 |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | 単位の完了率の値を取得します。 |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Primavera が使用するタスクの一意の識別子であるアクティビティ ID フィールドを取得します。

--------------------

アクティビティ（サマリタスク以外）にのみ適用されます。

**Returns:**
java.lang.String - アクティビティ ID フィールド - Primavera が使用するタスクの一意の識別子です。
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


「Activity Type」フィールドの値を取得します。

--------------------

アクティビティ（サマリタスク以外）にのみ適用されます。

**Returns:**
int - 'Activity Type' フィールドの値。
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


実際の経費コストの値を取得します。

**Returns:**
java.math.BigDecimal - 実際の費用コストの値。
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


実際の労働コストの値を取得します。

**Returns:**
java.math.BigDecimal - 実際の労働コストの値。
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


実際の労働単位の値を取得します。

**Returns:**
double - 実際の労働単位の値。
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


実際の材料コストの値を取得します。

**Returns:**
java.math.BigDecimal - 実際の材料コストの値。
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


実際の非労働単位の値を取得します。

**Returns:**
double - 実際の非労働単位の値。
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


実際の非労働コストの値を取得します。

**Returns:**
java.math.BigDecimal - 実際の非労働コストの値。
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


実際のコストの合計値を取得します。

**Returns:**
java.math.BigDecimal - 実際のコストの合計値。
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


予算（または計画）された経費コストの値を取得します。

**Returns:**
java.math.BigDecimal - 予算（または計画）された費用コストの値。
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


予算（または計画）された労働コストの値を取得します。

**Returns:**
java.math.BigDecimal - 予算（または計画）された労働コストの値。
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


予算（または計画）された材料コストの値を取得します。

**Returns:**
java.math.BigDecimal - 予算（または計画）された材料コストの値。
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


予算（または計画）された非労働コストの値を取得します。

**Returns:**
java.math.BigDecimal - 予算（または計画）された非労働コストの値。
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


予算（または計画）されたコストの合計値を取得します。

**Returns:**
java.math.BigDecimal - 予算（または計画）されたコストの合計値。
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


期間の完了率の値を取得します。

**Returns:**
double - 期間の完了率の値。
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


アクティビティの「Duration Type」フィールドの値を取得します。

--------------------

アクティビティ（サマリタスク以外）にのみ適用されます。

**Returns:**
int - アクティビティの 'Duration Type' フィールドの値。
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


アクティビティの「% Complete Type」フィールドの値を取得します。

--------------------

アクティビティ（サマリタスク以外）にのみ適用されます。

**Returns:**
int - アクティビティの '% Complete Type' フィールドの値。
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Physical Percent Complete の値を取得します。

--------------------

アクティビティ（サマリタスク以外）にのみ適用されます。

**Returns:**
double - 物理的完了率の値。
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


元のまたは計画された期間を取得します――タスクの計画開始日から計画終了日までの合計作業時間です。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


主要制約の日付を取得します。

**Returns:**
java.util.Date - 主な制約の日付。
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


主要制約のタイプを取得します。

**Returns:**
int - 主な制約のタイプ。
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


アクティビティの「Activity Type」フィールドの生テキスト表現（ソースファイル内の形式）を取得します。

--------------------

アクティビティ（サマリタスク以外）にのみ適用されます。

**Returns:**
java.lang.String - アクティビティの 'Activity Type' フィールドの（ソースファイル内の）生テキスト表現。
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


アクティビティの「% Complete Type」フィールドの生テキスト表現（ソースファイル内の形式）を取得します。

--------------------

アクティビティ（サマリタスク以外）にのみ適用されます。

**Returns:**
java.lang.String - アクティビティの '% Complete Type' フィールドの（ソースファイル内の）生テキスト表現。
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


アクティビティの「Duration Type」フィールドの生テキスト表現（ソースファイル内の形式）を取得します。

--------------------

アクティビティ（サマリタスク以外）にのみ適用されます。

**Returns:**
java.lang.String - アクティビティの 'Duration Type' フィールドの（ソースファイル内の）生テキスト表現。
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


アクティビティの「Status」フィールドの生テキスト表現（ソースファイル内の形式）を取得します。

--------------------

アクティビティ（サマリタスク以外）にのみ適用されます。

**Returns:**
java.lang.String - アクティビティの 'Status' フィールドの（ソースファイル内の）生テキスト表現。
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


残りの早期完了日を取得します――アクティビティの残作業が完了するように予定されている日付です。

**Returns:**
java.util.Date - 残りの早期完了日 - アクティビティの残り作業が完了するように予定されている日付。
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


残りの早期開始日を取得します――アクティビティの残作業が開始されるように予定されている日付です。

**Returns:**
java.util.Date - 残りの早期開始日 - アクティビティの残り作業が開始される予定の日付です。
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


残りの経費コストの値を取得します。

**Returns:**
java.math.BigDecimal - 残りの経費コストの値です。
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


残りの労働単位の値を取得します。

**Returns:**
double - 残りの労働単位の値です。
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


残りの遅延完了日を取得します。

**Returns:**
java.util.Date - 残りの遅延完了日です。
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


残りの遅延開始日を取得します。

**Returns:**
java.util.Date - 残りの遅延開始日です。
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


残りの非労働単位の値を取得します。

**Returns:**
double - 残りの非労働単位の値です。
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


二次制約の日付を取得します。

**Returns:**
java.util.Date - 二次制約の日付です。
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


二次制約のタイプを取得します。

**Returns:**
int - 二次制約のタイプです。
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


WBS項目（サマリタスク）のシーケンス番号を取得します。Primaveraでサマリタスクを並べ替えるために使用されます。

--------------------

WBS項目（サマリタスク）に適用可能です。

**Returns:**
int - WBS項目（サマリタスク）のシーケンス番号です。
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


単位の完了率の値を取得します。

**Returns:**
double - 完了率（パーセント）の単位値です。
