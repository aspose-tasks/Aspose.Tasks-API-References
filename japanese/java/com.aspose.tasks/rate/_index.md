---
title: "レート"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "リソースに対してその期間中に適用される時間期間とレートの定義を表します。"
type: docs
weight: 232
url: /ja/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

リソースに対してその期間中に適用される時間期間とレートの定義を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | リソースの使用ごとのコストを取得します。 |
| [getOvertimeRate()](#getOvertimeRate--) | リソースの時間あたりの残業率を取得します。 |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Microsoft Project が残業率を表示するために使用する単位を取得します。 |
| [getRateTable()](#getRateTable--) | リソースのレートテーブルの一意識別子を取得します。 |
| [getRatesFrom()](#getRatesFrom--) | レートが有効になる日付を取得します。 |
| [getRatesTo()](#getRatesTo--) | レートが有効である最終日付を取得します。 |
| [getStandardRate()](#getStandardRate--) | リソースの時間あたりの標準レートを取得します。 |
| [getStandardRateFormat()](#getStandardRateFormat--) | Microsoft Project が標準レートを表示するために使用する単位を取得します。 |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | リソースの使用ごとのコストを設定します。 |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | リソースの時間外料金（1時間あたり）を設定します。 |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Microsoft Project が時間外料金を表示する際に使用する単位を設定します。 |
| [setRateTable(int value)](#setRateTable-int-) | リソースのレートテーブルの一意識別子を設定します。 |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | レートが有効になる日付を設定します。 |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | レートが有効である最終日付を設定します。 |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | リソースの標準料金（1時間あたり）を設定します。 |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Microsoft Project が標準料金を表示する際に使用する単位を設定します。 |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


リソースの使用ごとのコストを取得します。レートテーブルがリソースに存在する場合、この値は現在の日付から取得されます。

**Returns:**
java.math.BigDecimal - リソースの使用ごとのコスト。
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


リソースの時間あたりの残業率を取得します。

**Returns:**
java.math.BigDecimal - リソースの時間外料金（1時間あたり）。
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Microsoft Project が残業率を表示するために使用する単位を取得します。

**Returns:**
int - Microsoft Project が時間外料金を表示する際に使用する単位。
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


リソースのレートテーブルの一意識別子を取得します。

**Returns:**
int - リソースのレートテーブルの一意識別子。
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


レートが有効になる日付を取得します。

**Returns:**
java.util.Date - レートが有効になる日付。
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


レートが有効である最終日付を取得します。

**Returns:**
java.util.Date - レートが有効である最終日付。
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


リソースの時間あたりの標準レートを取得します。

**Returns:**
java.math.BigDecimal - リソースの標準料金（1時間あたり）。
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Microsoft Project が標準レートを表示するために使用する単位を取得します。

**Returns:**
int - Microsoft Project が標準料金を表示する際に使用する単位。
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


リソースの使用ごとのコストを設定します。レートテーブルがリソースに存在する場合、この値は現在の日付から取得されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | リソースの使用ごとのコスト。 |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


リソースの時間外料金（1時間あたり）を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | リソースの時間外料金（1時間あたり）。 |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Microsoft Project が時間外料金を表示する際に使用する単位を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Microsoft Project が時間外料金を表示する際に使用する単位。 |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


リソースのレートテーブルの一意識別子を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | リソースのレートテーブルの一意識別子。 |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


レートが有効になる日付を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | レートが有効になる日付。 |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


レートが有効である最終日付を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | レートが有効である最終日付。 |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


リソースの標準料金（1時間あたり）を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | リソースの標準料金（1時間あたり）。 |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Microsoft Project が標準料金を表示する際に使用する単位を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Microsoft Project が標準料金を表示するために使用する単位。 |

