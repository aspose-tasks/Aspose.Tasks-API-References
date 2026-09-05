---
title: "GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "グラフィカル インジケータ基準の条件チェックで使用される値を表します。"
type: docs
weight: 117
url: /ja/java/com.aspose.tasks/graphicalindicatorcriteriavalue/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteriaValue
```

グラフィカル インジケータ基準の条件チェックで使用される値を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [GraphicalIndicatorCriteriaValue(BigDecimal value)](#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-) | 定数の BigDecimal 値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。 |
| [GraphicalIndicatorCriteriaValue(Date dateValue)](#GraphicalIndicatorCriteriaValue-java.util.Date-) | 定数の Date 値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。 |
| [GraphicalIndicatorCriteriaValue(String textValue)](#GraphicalIndicatorCriteriaValue-java.lang.String-) | 定数の String 値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。 |
| [GraphicalIndicatorCriteriaValue(Duration durationValue)](#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-) | 定数の Duration 値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。 |
| [GraphicalIndicatorCriteriaValue(boolean flagValue)](#GraphicalIndicatorCriteriaValue-boolean-) | 定数のフラグ（boolean）値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [createFieldLink(int field)](#createFieldLink-int-) | 指定された MS Project のフィールドの値を表す GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。 |
| [getRawValue()](#getRawValue--) | フィールド値の基になる定数を取得します。 |
| [isFieldLink()](#isFieldLink--) | 現在のインスタンスがフィールドリンクかどうか（フィールドの値を表すか）を取得します。 |
| [toString()](#toString--) | 現在のオブジェクトを表す文字列を返します。 |
### GraphicalIndicatorCriteriaValue(BigDecimal value) {#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-}
```
public GraphicalIndicatorCriteriaValue(BigDecimal value)
```


定数の BigDecimal 値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | BigDecimal 値 |

### GraphicalIndicatorCriteriaValue(Date dateValue) {#GraphicalIndicatorCriteriaValue-java.util.Date-}
```
public GraphicalIndicatorCriteriaValue(Date dateValue)
```


定数の Date 値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dateValue | java.util.Date | Date 値 |

### GraphicalIndicatorCriteriaValue(String textValue) {#GraphicalIndicatorCriteriaValue-java.lang.String-}
```
public GraphicalIndicatorCriteriaValue(String textValue)
```


定数の String 値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| textValue | java.lang.String | String 値 |

### GraphicalIndicatorCriteriaValue(Duration durationValue) {#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-}
```
public GraphicalIndicatorCriteriaValue(Duration durationValue)
```


定数の Duration 値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | Duration 値 |

### GraphicalIndicatorCriteriaValue(boolean flagValue) {#GraphicalIndicatorCriteriaValue-boolean-}
```
public GraphicalIndicatorCriteriaValue(boolean flagValue)
```


定数のフラグ（boolean）値を持つ GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| flagValue | boolean | フラグ（boolean）値 |

### createFieldLink(int field) {#createFieldLink-int-}
```
public static GraphicalIndicatorCriteriaValue createFieldLink(int field)
```


指定された MS Project のフィールドの値を表す GraphicalIndicatorCriteriaValue クラスのインスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| フィールド | int | 指定されたフィールド |

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - instance of GraphicalIndicatorCriteriaValue class representing the value of the specified field
### getRawValue() {#getRawValue--}
```
public final Object getRawValue()
```


フィールド値の基になる定数を取得します。

**Returns:**
java.lang.Object - フィールド値の基になる定数
### isFieldLink() {#isFieldLink--}
```
public final boolean isFieldLink()
```


現在のインスタンスがフィールドリンクかどうか（フィールドの値を表すか）を取得します。

**Returns:**
boolean - 現在のインスタンスがフィールドリンクかどうか（フィールドの値を表すか）
### toString() {#toString--}
```
public String toString()
```


現在のオブジェクトを表す文字列を返します。

**Returns:**
java.lang.String - 現在のオブジェクトを表す文字列
