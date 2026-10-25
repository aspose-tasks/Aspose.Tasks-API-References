---
title: "Duration"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクト内の期間を表します。"
type: docs
weight: 76
url: /ja/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

プロジェクト内の期間を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [Duration()](#Duration--) | 指定された TimeSpan 値と TimeUnitType を使用して、[Duration](../../com.aspose.tasks/duration) 構造体の新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [Clone()](#Clone--) | このインスタンスのディープコピーを作成して返します。 |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | インスタンスのディープコピーを別のインスタンスに作成します。 |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | 指定された期間をこの期間に加算します。 |
| [add(double val)](#add-double-) | 指定された double 値をこの期間に加算します。 |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Duration オブジェクトを、指定された時間単位の別の期間に変換します。 |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | 指定された `obj1` インスタンスが指定された `obj2` インスタンスと等しいかどうかを示す値を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getTimeSpan()](#getTimeSpan--) | この Duration オブジェクトの `TimeSpan` インスタンスを取得します（[getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-))。 |
| [getTimeUnit()](#getTimeUnit--) | このオブジェクトの時間単位タイプを取得します。 |
| [hashCode()](#hashCode--) | このオブジェクトのハッシュコード値を返します。 |
| [isElapsed()](#isElapsed--) | 時間単位が経過かどうかを示す値を取得します。 |
| [isEstimated()](#isEstimated--) | 時間単位が推定かどうかを示す値を取得します。 |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値を返します。 |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | 指定された文字列を [Duration](../../com.aspose.tasks/duration) 構造体のインスタンスに変換します。 |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | フォーマット "PT--H--M--S--" の期間文字列を解析します。 |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | 指定された期間をこの期間インスタンスから減算します。 |
| [subtract(double val)](#subtract-double-) | 指定された double 値をこの期間インスタンスから減算します。 |
| [toDouble()](#toDouble--) | Duration オブジェクトを `double` 値に変換します。 |
| [toString()](#toString--) | このインスタンスの文字列表現を返します。 |
### Duration() {#Duration--}
```
public Duration()
```


指定された TimeSpan 値と TimeUnitType を使用して、[Duration](../../com.aspose.tasks/duration) 構造体の新しいインスタンスを初期化します。

### Clone() {#Clone--}
```
public Duration Clone()
```


このインスタンスのディープコピーを作成して返します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


インスタンスのディープコピーを別のインスタンスに作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | 別のインスタンス。 |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


指定された期間をこの期間に加算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | このインスタンスに追加する指定された[Duration](../../com.aspose.tasks/duration)。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


指定された double 値をこの期間に加算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| val | double | このインスタンスに追加する指定された`double`値。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


Duration オブジェクトを、指定された時間単位の別の期間に変換します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| timeUnitType | バイト | 指定された時間単位の種類。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | このインスタンスと比較するオブジェクトです。 |

**Returns:**
boolean - このインスタンスと同じ TimeSpan と TimeUnit の値を持つ他の Duration インスタンスがある場合は **True** を返し、そうでない場合は **false** を返します。
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


指定された `obj1` インスタンスが指定された `obj2` インスタンスと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | 比較する最初のオブジェクト。 |
| obj2 | [Duration](../../com.aspose.tasks/duration) | 比較する2番目のオブジェクト。 |

**Returns:**
boolean - 指定された `obj1` インスタンスが指定された `obj2` インスタンスと等しい場合は true を返し、そうでない場合は false を返します。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するオブジェクトです。 |

**Returns:**
boolean - 指定されたオブジェクトがこのインスタンスと同じ TimeSpan と TimeUnit の値を持つ Duration の場合は **True**、それ以外の場合は **false** を返します。
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


この Duration オブジェクトの `TimeSpan` インスタンスを取得します（[getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-))。

Value: この Duration オブジェクトの TimeSpan インスタンス。

**Returns:**
double - この Duration オブジェクトの `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) インスタンス。
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


このオブジェクトの時間単位タイプを取得します。

Value: この Duration インスタンスの時間単位の種類。

**Returns:**
byte - このオブジェクトの時間単位の種類。
### hashCode() {#hashCode--}
```
public int hashCode()
```


このオブジェクトのハッシュコード値を返します。

**Returns:**
int - この Duration インスタンスのハッシュコード値を返します。
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


時間単位が経過かどうかを示す値を取得します。

Value: この Duration インスタンスが経過しているかどうかを示すフラグ。

**Returns:**
boolean - 時間単位が経過しているかどうかを示す値。
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


時間単位が推定かどうかを示す値を取得します。

Value: この Duration インスタンスが推定であるかどうかを示すフラグ。

**Returns:**
boolean - 時間単位が推定であるかどうかを示す値。
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | 最初の期間。 |
| b | [Duration](../../com.aspose.tasks/duration) | 2番目の期間。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しいかどうかを示す値
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | 最初の期間。 |
| b | [Duration](../../com.aspose.tasks/duration) | 2番目の期間。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


指定された文字列を [Duration](../../com.aspose.tasks/duration) 構造体のインスタンスに変換します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | 期間を変換するための指定された[Project](../../com.aspose.tasks/project)クラスのインスタンス。 |
| 値 | java.lang.String | 変換する指定された文字列。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


フォーマット "PT--H--M--S--" の期間文字列を解析します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 解析する指定された文字列。 |

**Returns:**
double - 解析された `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) 構造体のインスタンスを返します。
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


指定された期間をこの期間インスタンスから減算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | このインスタンスから減算する指定された[Duration](../../com.aspose.tasks/duration)インスタンス。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


指定された double 値をこの期間インスタンスから減算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| val | double | このインスタンスから減算する指定された`double`値。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Duration オブジェクトを `double` 値に変換します。

**Returns:**
double - 変換された値。
### toString() {#toString--}
```
public String toString()
```


このインスタンスの文字列表現を返します。

**Returns:**
java.lang.String - このインスタンスの文字列表現です。
