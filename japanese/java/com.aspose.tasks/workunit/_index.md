---
title: "WorkUnit"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "作業時間を表します。"
type: docs
weight: 362
url: /ja/java/com.aspose.tasks/workunit/
---

**Inheritance:**
java.lang.Object
```
public class WorkUnit
```

作業時間を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [WorkUnit(Date from, Date to)](#WorkUnit-java.util.Date-java.util.Date-) | 新しい [WorkUnit](../../com.aspose.tasks/workunit) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getFrom()](#getFrom--) | From 日付を取得します。 |
| [getTo()](#getTo--) | To 日付を取得します。 |
| [getWorkingHours()](#getWorkingHours--) | 作業時間の期間を取得します。 |
| [setFrom(Date value)](#setFrom-java.util.Date-) | From 日付を設定します。 |
| [setTo(Date value)](#setTo-java.util.Date-) | To 日付を設定します。 |
| [setWorkingHours(double value)](#setWorkingHours-double-) | 作業時間の期間を設定します。 |
### WorkUnit(Date from, Date to) {#WorkUnit-java.util.Date-java.util.Date-}
```
public WorkUnit(Date from, Date to)
```


新しい [WorkUnit](../../com.aspose.tasks/workunit) クラスのインスタンスを初期化します。指定された From と To の日付で新しい WorkUnit オブジェクトを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| from | java.util.Date | 作業時間の開始日。 |
| to | java.util.Date | 作業時間の終了日。 |

### getFrom() {#getFrom--}
```
public final Date getFrom()
```


From 日付を取得します。

**Returns:**
java.util.Date - From 日付。
### getTo() {#getTo--}
```
public final Date getTo()
```


To 日付を取得します。

**Returns:**
java.util.Date - 終了日。
### getWorkingHours() {#getWorkingHours--}
```
public final double getWorkingHours()
```


作業時間の期間を取得します。

**Returns:**
double - 勤務時間の期間。
### setFrom(Date value) {#setFrom-java.util.Date-}
```
public void setFrom(Date value)
```


From 日付を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 開始日。 |

### setTo(Date value) {#setTo-java.util.Date-}
```
public final void setTo(Date value)
```


To 日付を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 終了日。 |

### setWorkingHours(double value) {#setWorkingHours-double-}
```
public final void setWorkingHours(double value)
```


作業時間の期間を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | 勤務時間の期間。 |

