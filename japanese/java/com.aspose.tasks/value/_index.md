---
title: "値"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "値リスト内の値を表します。"
type: docs
weight: 333
url: /ja/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

値リスト内の値を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [Value()](#Value--) | 新しい [Value](../../com.aspose/tasks/value) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDateValue()](#getDateValue--) | DateTime として表現できる場合、実際の値を取得します。 |
| [getDescription()](#getDescription--) | 値の説明を取得します。 |
| [getDuration()](#getDuration--) | Duration を表すために使用される実際の値を取得します。 |
| [getId()](#getId--) | プロジェクト全体での値の一意の識別子を取得します。 |
| [getNumericValue()](#getNumericValue--) | 数値またはコスト値を表すために使用される実際の値を取得します。 |
| [getPhonetic()](#getPhonetic--) | カスタムフィールド名に関する音韻情報を取得します。 |
| [getStringValue()](#getStringValue--) | テキスト文字列を表すために使用される実際の値を取得します。 |
| [getVal()](#getVal--) | 内部表現の実際の値を取得します。 |
| [getValueGuid()](#getValueGuid--) | プロジェクト全体で他の値と区別する GUID を取得します。 |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | DateTime として表現できる場合、実際の値を設定します。 |
| [setDescription(String value)](#setDescription-java.lang.String-) | 値の説明を設定します。 |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Duration を表すために使用される実際の値を設定します。 |
| [setId(int value)](#setId-int-) | プロジェクト全体での値の一意の識別子を設定します。 |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | 数値またはコスト値を表すために使用される実際の値を設定します。 |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | カスタムフィールド名に関する音韻情報を設定します。 |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | テキスト文字列を表すために使用される実際の値を設定します。 |
| [setVal(String value)](#setVal-java.lang.String-) | 内部表現の実際の値を設定します。 |
### Value() {#Value--}
```
public Value()
```


新しい [Value](../../com.aspose/tasks/value) クラスのインスタンスを初期化します。

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


DateTime として表現できる場合、実際の値を取得します。デフォルト値は DateTime\#MinValue.MinValue です。

--------------------

DateTime の値を設定する必要がある場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) よりこのプロパティを使用してください。

**Returns:**
java.util.Date - DateTime として表現できる場合の実際の値。
### getDescription() {#getDescription--}
```
public final String getDescription()
```


値の説明を取得します。

**Returns:**
java.lang.String - 値の説明。
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Duration を表すために使用される実際の値を取得します。

--------------------

Duration の値を設定する必要がある場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) よりこのプロパティを使用してください。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


プロジェクト全体での値の一意の識別子を取得します。

異なる [Value](../../com.aspose.tasks/value) インスタンスに同じ識別子を使用しないことが重要です。

最小の `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) の値は `1` です。

**Returns:**
int - プロジェクト全体での値の一意の識別子。
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


数値またはコスト値を表すために使用される実際の値を取得します。

--------------------

Number または Cost の値を設定する必要がある場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) よりこのプロパティを使用してください。

**Returns:**
java.math.BigDecimal - 数値またはコスト値を表すために使用される実際の値。
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


カスタムフィールド名に関する音韻情報を取得します。

**Returns:**
java.lang.String - カスタムフィールド名に関する音韻情報。
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


テキスト文字列を表すために使用される実際の値を取得します。

--------------------

Text の値を設定する必要がある場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) よりこのプロパティを使用してください。

**Returns:**
java.lang.String - Text 文字列を表すために使用される実際の値。
### getVal() {#getVal--}
```
public final String getVal()
```


内部表現での実際の値を取得します。以下に一覧された強く型付けされたプロパティの使用を推奨します。

--------------------

Text の値を設定したい場合は、強く型付けされた `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) プロパティの使用を推奨します。

Number または Cost の値を設定したい場合は、強く型付けされた `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) プロパティの使用を推奨します。

Date/Start/Finish の値を設定したい場合は、強く型付けされた `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) プロパティの使用を推奨します。

Duration の値を設定したい場合は、強く型付けされた `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) プロパティの使用を推奨します。

タイプが一覧にない場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) プロパティを使用してください。

**Returns:**
java.lang.String - 内部表現での実際の値。
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


プロジェクト全体で他の値と区別する GUID を取得します。

**Returns:**
java.util.UUID - プロジェクト全体でこの値を他と区別する GUID。
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


DateTime として表現できる場合は実際の値を設定します。デフォルト値は DateTime\#MinValue.MinValue です。

--------------------

DateTime の値を設定する必要がある場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) よりこのプロパティを使用してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | DateTime として表現できる場合の実際の値。 |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


値の説明を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 値の説明。 |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Duration を表すために使用される実際の値を設定します。

--------------------

Duration の値を設定する必要がある場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) よりこのプロパティを使用してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Duration を表すために使用される実際の値。 |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


プロジェクト全体での値の一意の識別子を設定します。

異なる [Value](../../com.aspose.tasks/value) インスタンスに同じ識別子を使用しないことが重要です。

最小の `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) の値は `1` です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | プロジェクト全体での値の一意の識別子です。 |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


数値またはコスト値を表すために使用される実際の値を設定します。

--------------------

Number または Cost の値を設定する必要がある場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) よりこのプロパティを使用してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | 数値またはコスト値を表すために使用される実際の値です。 |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


カスタムフィールド名に関する音韻情報を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | カスタム フィールド名に関する音韻情報です。 |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


テキスト文字列を表すために使用される実際の値を設定します。

--------------------

Text の値を設定する必要がある場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) よりこのプロパティを使用してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | テキスト文字列を表すために使用される実際の値です。 |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


内部表現で実際の値を設定します。以下に一覧されている強く型付けされたプロパティの使用を推奨します。

--------------------

Text の値を設定したい場合は、強く型付けされた `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) プロパティの使用を推奨します。

Number または Cost の値を設定したい場合は、強く型付けされた `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) プロパティの使用を推奨します。

Date/Start/Finish の値を設定したい場合は、強く型付けされた `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) プロパティの使用を推奨します。

Duration の値を設定したい場合は、強く型付けされた `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) プロパティの使用を推奨します。

タイプが一覧にない場合は、`Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) プロパティを使用してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 内部表現の実際の値です。 |

