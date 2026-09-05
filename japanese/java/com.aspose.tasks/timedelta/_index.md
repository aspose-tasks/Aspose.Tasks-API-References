---
title: "TimeDelta"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "2 つのタイムスタンプ間の差分を表します。"
type: docs
weight: 317
url: /ja/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

2 つのタイムスタンプ間の差分を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | 指定された時間、分、秒の数で TimeDelta の新しいインスタンスを初期化します。 |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | 指定された日数、時間、分、秒、ミリ秒の数で TimeDelta の新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | このインスタンスと他のインスタンスの合計値を持つ新しい TimeDelta オブジェクトを返します。 |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | 2 つの TimeDelta 値を比較し、最初の値が 2 番目の値より短いか、等しいか、長いかを示す整数を返します。 |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | このインスタンスを指定された TimeDelta オブジェクトと比較し、インスタンスが TimeSpan オブジェクトより短いか、等しいか、長いかを示す整数を返します。 |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | `other` の時間スパンがこれと等しいかどうかを示します。 |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | 2 つのインスタンスが等しいかどうかをチェックします。 |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | 指定された日数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。 |
| [fromHours(double value)](#fromHours-double-) | 指定された時間数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。 |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | 指定されたミリ秒数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。 |
| [fromMinutes(double value)](#fromMinutes-double-) | 指定された分数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。 |
| [fromSeconds(double value)](#fromSeconds-double-) | 指定された秒数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。 |
| [getDays()](#getDays--) | このインスタンスが表す時間間隔の日コンポーネントを返します。 |
| [getHours()](#getHours--) | このインスタンスが表す時間間隔の時間コンポーネントを返します。 |
| [getMilliseconds()](#getMilliseconds--) | このインスタンスが表す時間間隔のミリ秒コンポーネントを返します。 |
| [getMinutes()](#getMinutes--) | このインスタンスで表される時間間隔の分コンポーネントを返します。 |
| [getSeconds()](#getSeconds--) | このインスタンスで表される時間間隔の秒コンポーネントを返します。 |
| [getTotalDays()](#getTotalDays--) | 現在のインスタンスの値を整数日と小数日で表したものを返します。 |
| [getTotalHours()](#getTotalHours--) | 現在のインスタンスの値を整数時間と小数時間で表したものを返します。 |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | 現在のインスタンスの値を整数ミリ秒と小数ミリ秒で表したものを返します。 |
| [getTotalMinutes()](#getTotalMinutes--) | 現在のインスタンスの値を整数分と小数分で表したものを返します。 |
| [getTotalSeconds()](#getTotalSeconds--) | 現在のインスタンスの値を整数秒と小数秒で表したものを返します。 |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | このインスタンスの値を否定した値を持つ新しい `TimeDelta` を返します。 |
| [parse(String s)](#parse-java.lang.String-) | 時間間隔の文字列表現を `TimeDelta` に変換します。 |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | このインスタンスと `other` インスタンスの差分を値とする新しい TimeDelta オブジェクトを返します。 |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | 時間間隔の文字列表現を TimeDelta に変換し、変換が成功したかどうかを示す値を返します。 |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


指定された時間、分、秒の数で TimeDelta の新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 時間 | int | 時間数。 |
| 分 | int | 分数。 |
| 秒 | int | 秒数。 |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


指定された日数、時間、分、秒、ミリ秒の数で TimeDelta の新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 日 | int | 日数。 |
| 時間 | int | 時間数。 |
| 分 | int | 分数。 |
| 秒 | int | 秒数。 |
| ミリ秒 | int | ミリ秒数。 |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


このインスタンスと他のインスタンスの合計値を持つ新しい TimeDelta オブジェクトを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 合計するインスタンス。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


2 つの TimeDelta 値を比較し、最初の値が 2 番目の値より短いか、等しいか、長いかを示す整数を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | 比較する最初の時間間隔。 |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | 比較する二番目の時間間隔。 |

**Returns:**
int - \-1 は `t1` が `t2` より短い場合、0 は `t1` が `t2` と等しい場合、1 は `t1` が `t2` より長い場合を示します。
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


このインスタンスを指定された TimeDelta オブジェクトと比較し、インスタンスが TimeSpan オブジェクトより短いか、等しいか、長いかを示す整数を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 比較対象となるインスタンス。 |

**Returns:**
int - \-1 このインスタンスが `other` より短い場合、`other` と等しい場合は 0、`other` より長い場合は 1。
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


`other` の時間スパンがこれと等しいかどうかを示します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 比較対象となる時間間隔。 |

**Returns:**
boolean - `true` が間隔が等しい場合; `false` はそれ以外。
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


2 つのインスタンスが等しいかどうかをチェックします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | 最初のインスタンス。 |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | 2番目のインスタンス。 |

**Returns:**
boolean - `true` がインスタンスが等しい場合; `false` はそれ以外。
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 他 | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


指定された日数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | 日数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


指定された時間数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | 時間数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


指定されたミリ秒数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | ミリ秒数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


指定された分数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | 分数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


指定された秒数（最も近いミリ秒に丸めた）を表す TimeDelta を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | 秒数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


このインスタンスが表す時間間隔の日コンポーネントを返します。

**Returns:**
int - 時間間隔の「日」コンポーネント。正または負になる可能性があります。
### getHours() {#getHours--}
```
public int getHours()
```


このインスタンスが表す時間間隔の時間コンポーネントを返します。

**Returns:**
int - 時間間隔の時間コンポーネント（-23 から 23 の範囲）。
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


このインスタンスが表す時間間隔のミリ秒コンポーネントを返します。

**Returns:**
int - 時間間隔のミリ秒コンポーネント（-999 から 999 の範囲）。
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


このインスタンスで表される時間間隔の分コンポーネントを返します。

**Returns:**
int - 時間間隔の分コンポーネント（-59 から 59 の範囲）。
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


このインスタンスで表される時間間隔の秒コンポーネントを返します。

**Returns:**
int - 時間間隔の秒コンポーネント（-59 から 59 の範囲）。
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


現在のインスタンスの値を整数日と小数日で表したものを返します。

**Returns:**
double - このインスタンスが表す総日数。
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


現在のインスタンスの値を整数時間と小数時間で表したものを返します。

**Returns:**
double - このインスタンスが表す総時間数。
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


現在のインスタンスの値を整数ミリ秒と小数ミリ秒で表したものを返します。

**Returns:**
double - このインスタンスが表す総ミリ秒数。
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


現在のインスタンスの値を整数分と小数分で表したものを返します。

**Returns:**
double - このインスタンスが表す総分数。
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


現在のインスタンスの値を整数秒と小数秒で表したものを返します。

**Returns:**
double - このインスタンスが表す総秒数。
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


このインスタンスの値を否定した値を持つ新しい `TimeDelta` を返します。

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


時間間隔の文字列表現を `TimeDelta` に変換します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| s | java.lang.String | 変換する時間間隔を指定する文字列。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


このインスタンスと `other` インスタンスの差分を値とする新しい TimeDelta オブジェクトを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 減算するインスタンス。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


時間間隔の文字列表現を TimeDelta に変換し、変換が成功したかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| s | java.lang.String | 変換する時間間隔を指定する文字列。 |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | この配列は少なくとも1つの要素を含んでいる必要があります。このメソッドが戻ると、`result[0]` には `s` で指定された時間間隔を表すオブジェクト、または変換に失敗した場合は長さ0の時間間隔が含まれます。 |

**Returns:**
boolean - 変換が成功した場合は `true`、それ以外は `false`。
