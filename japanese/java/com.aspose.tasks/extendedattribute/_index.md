---
title: "ExtendedAttribute"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "拡張属性を表します。"
type: docs
weight: 81
url: /ja/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

拡張属性を表します。

--------------------

現在、MSP Xml 2003/2007 および mpp 2003 からのすべてのタイプの拡張属性の読み取りがサポートされています。MSP mpp 2007 では、期間とフラグを除くすべての拡張属性の読み取りがサポートされています。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | 属性定義を取得します。 |
| [getDateValue()](#getDateValue--) | 日付タイプ（Date、Start、Finish）の属性の値を取得します。 |
| [getDurationValue()](#getDurationValue--) | 「Duration」タイプの属性の値を取得します。 |
| [getFieldId()](#getFieldId--) | フィールドのIDを取得します。 |
| [getFlagValue()](#getFlagValue--) | 「Flag」タイプの属性にフラグが設定されているかどうかを示す値を取得します。 |
| [getNumericValue()](#getNumericValue--) | 数値タイプ（Cost、Number）の属性の値を取得します。 |
| [getTextValue()](#getTextValue--) | 「Text」タイプの属性の値を取得します。 |
| [getValueGuid()](#getValueGuid--) | ルックアップ値のGUIDを取得します。 |
| [getValueReadOnly()](#getValueReadOnly--) | この[ExtendedAttribute](../../com.aspose.tasks/extendedattribute)インスタンスの値が読み取り専用かどうかを示す値を取得します。 |
| [isErrorValue()](#isErrorValue--) | 拡張属性の値の計算がエラーになったかどうかを取得します。 |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | 日付タイプ（Date、Start、Finish）の属性に値を設定します。 |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | 'Duration' 型の属性の値を設定します。 |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | 'Flag' 型の属性にフラグが設定されているかを示す値を設定します。 |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | 数値型（Cost、Number）の属性の値を設定します。 |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | 'Text' 型の属性の値を設定します。 |
| [toString()](#toString--) | 拡張属性の短い文字列表現を返します。 |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


属性定義を取得します。

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


日付タイプ（Date、Start、Finish）の属性の値を取得します。

**Returns:**
java.util.Date - 日付型（Date、Start、Finish）の属性の値です。
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


「Duration」タイプの属性の値を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


フィールドのIDを取得します。

**Returns:**
java.lang.String - フィールドの ID です。
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


「Flag」タイプの属性にフラグが設定されているかどうかを示す値を取得します。

**Returns:**
boolean - 'Flag' 型の属性にフラグが設定されているかを示す値です。
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


数値タイプ（Cost、Number）の属性の値を取得します。

**Returns:**
java.math.BigDecimal - 数値型（Cost、Number）の属性の値です。
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


「Text」タイプの属性の値を取得します。

**Returns:**
java.lang.String - 'Text' 型の属性の値です。
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


ルックアップ値のGUIDを取得します。

--------------------

直接設定すべきではなく、代わりに ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) を使用して、ルックアップ値を持つ拡張属性を作成してください。

**Returns:**
java.lang.String - ルックアップ値の GUID です。
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


この[ExtendedAttribute](../../com.aspose.tasks/extendedattribute)インスタンスの値が読み取り専用かどうかを示す値を取得します。

Value: このオブジェクトの [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) に数式またはロールアップが定義されている場合、true を返します。

**Returns:**
boolean - この [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) インスタンスの値が読み取り専用かどうかを示す値です。
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


拡張属性の値の計算がエラーになったかどうかを取得します。

**Returns:**
boolean - 拡張属性の値の計算がエラーになったかどうかです。
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


日付タイプ（Date、Start、Finish）の属性に値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 日付型（Date、Start、Finish）の属性の値です。 |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


'Duration' 型の属性の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 'Duration' 型の属性の値です。 |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


'Flag' 型の属性にフラグが設定されているかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 'Flag' 型の属性にフラグが設定されているかを示す値です。 |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


数値型（Cost、Number）の属性の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | 数値型（Cost、Number）の属性の値です。 |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


'Text' 型の属性の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 'Text' 型の属性の値です。 |

### toString() {#toString--}
```
public String toString()
```


拡張属性の短い文字列表現を返します。

**Returns:**
java.lang.String - 拡張属性の文字列表現です。
