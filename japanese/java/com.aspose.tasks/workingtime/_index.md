---
title: "WorkingTime"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "平日中の作業時間を表します。"
type: docs
weight: 365
url: /ja/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

平日中の作業時間を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | 指定された開始時刻と終了時刻を持つ間隔で、[WorkingTime](../../com.aspose.tasks/workingtime) クラスの新しいインスタンスを初期化します。 |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | 指定された開始時刻と終了時刻を持つ間隔項目で、[WorkingTime](../../com.aspose.tasks/workingtime) クラスの新しいインスタンスを初期化します。 |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | 指定された開始時刻と終了時刻を持つ間隔項目で、[WorkingTime](../../com.aspose.tasks/workingtime) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | オブジェクトが等しいかどうかをチェックします。 |
| [getFrom()](#getFrom--) | 作業時間の開始時刻を取得します。 |
| [getTo()](#getTo--) | 作業時間の終了時刻を取得します。 |
| [hashCode()](#hashCode--) | [WorkingTime](../../com.aspose.tasks/workingtime) クラスのインスタンスのハッシュコード値を返します。 |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


指定された開始時刻と終了時刻を持つ間隔で、[WorkingTime](../../com.aspose.tasks/workingtime) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fromTime | java.util.Date | 間隔の開始時刻 |
| toTime | java.util.Date | 間隔の終了時刻 |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


指定された開始時刻と終了時刻を持つ間隔項目で、[WorkingTime](../../com.aspose.tasks/workingtime) クラスの新しいインスタンスを初期化します。

--------------------

&gt; ```
&gt; WorkingTime コンストラクタのオーバーロードを使用して、TimeSpan を用いて間隔の開始と終了を初期化できます：
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fromHours | int | 間隔の開始時刻は、0〜24 の整数時間で表されます。 |
| toHours | int | 間隔の終了時刻は、0〜24 の整数時間で表されます。 |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


オブジェクトが等しいかどうかをチェックします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | 比較対象の第2オブジェクト。 |

**Returns:**
boolean - オブジェクトが等しい場合は true、そうでない場合は false。
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


作業時間の開始時刻を取得します。

**Returns:**
java.util.Date - 作業時間の開始時刻。
### getTo() {#getTo--}
```
public final Date getTo()
```


作業時間の終了時刻を取得します。

**Returns:**
java.util.Date - 作業時間の終了時刻。
### hashCode() {#hashCode--}
```
public int hashCode()
```


[WorkingTime](../../com.aspose.tasks/workingtime) クラスのインスタンスのハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
