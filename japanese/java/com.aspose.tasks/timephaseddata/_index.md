---
title: "TimephasedData"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "時間フェーズデータを表します。"
type: docs
weight: 320
url: /ja/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

時間フェーズデータを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | 新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | コストベースの時間フェーズデータ用に、新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを作成し、初期化します。 |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | コストベースの時間フェーズデータ用に、新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを作成し、初期化します。 |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | 素材リソースの割り当ての単位ベース時間フェーズデータ用に、新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを作成し、初期化します。 |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | 作業ベースの時間フェーズデータ用に、新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを作成し、初期化します。 |
| [getFinish()](#getFinish--) | 時間フェーズデータ期間の終了日を取得します。 |
| [getStart()](#getStart--) | 時間フェーズデータ期間の開始日を取得します。 |
| [getTimephasedDataType()](#getTimephasedDataType--) | 時間フェーズデータのタイプを取得します。 |
| [getUid()](#getUid--) | 時間フェーズデータの一意識別子を取得します |
| [getUnit()](#getUnit--) | 時間フェーズデータ期間の時間単位を取得します。 |
| [getValue()](#getValue--) | 時間フェーズデータ期間の時間単位あたりの値を取得します。 |
| [getValueToCost()](#getValueToCost--) | `double` インスタンスを取得します。このオブジェクトの文字列値を表します。 |
| [getValueToDuration()](#getValueToDuration--) | double インスタンスを取得します。このオブジェクトの文字列値を表します。 |
| [getValueToUnits()](#getValueToUnits--) | `double` インスタンスを取得します。このオブジェクトの文字列値を、単位ベースの時間フェーズデータ用に表します。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | 時間フェーズデータ期間の終了日を設定します。 |
| [setStart(Date value)](#setStart-java.util.Date-) | 時間フェーズデータ期間の開始日を設定します。 |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | 時間フェーズデータのタイプを設定します。 |
| [setUid(int value)](#setUid-int-) | 時間フェーズデータの一意識別子を設定します |
| [setUnit(byte value)](#setUnit-byte-) | 時間フェーズデータ期間の時間単位を設定します。 |
| [setValue(String value)](#setValue-java.lang.String-) | 時間フェーズデータ期間の時間単位あたりの値を設定します。 |
| [setValueToCost(double value)](#setValueToCost-double-) | `double` インスタンスは、このオブジェクトの文字列値を表します。 |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを初期化します。

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


コストベースの時間フェーズデータ用に、新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを作成し、初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| uid | int | タスクの UID。 |
| 開始 | java.util.Date | 開始日時。 |
| 終了 | java.util.Date | 終了日時。 |
| 値 | double | コスト値。 |
| type | バイト | 時間フェーズデータのタイプ。 |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


コストベースの時間フェーズデータ用に、新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを作成し、初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| uid | int | タスクの UID。 |
| 開始 | java.util.Date | 開始日時。 |
| 終了 | java.util.Date | 終了日時。 |
| 値 | double | コスト値。 |
| timeUnit | バイト | 時間単位のタイプ。 |
| type | バイト | 時間フェーズデータのタイプ。 |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


素材リソースの割り当ての単位ベース時間フェーズデータ用に、新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを作成し、初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| uid | int | タスクの UID。 |
| 開始 | java.util.Date | 開始日時。 |
| 終了 | java.util.Date | 終了日時。 |
| 単位 | double | 単位数。 |
| type | バイト | 時間フェーズデータのタイプ。 |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


作業ベースの時間フェーズデータ用に、新しい [TimephasedData](../../com.aspose.tasks/timephaseddata) クラスのインスタンスを作成し、初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| uid | int | タスクの UID。 |
| 開始 | java.util.Date | 開始日時。 |
| 終了 | java.util.Date | 終了日時。 |
| 値 | double | 時間間隔の値。 |
| timeUnit | バイト | 時間単位のタイプ。 |
| type | バイト | 時間フェーズデータのタイプ。 |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


時間フェーズデータ期間の終了日を取得します。

**Returns:**
java.util.Date - 時間フェーズデータ期間の終了日。
### getStart() {#getStart--}
```
public final Date getStart()
```


時間フェーズデータ期間の開始日を取得します。

**Returns:**
java.util.Date - 時間フェーズデータ期間の開始日。
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


時間フェーズデータのタイプを取得します。

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) プロパティは、ここで指定された型に適さない場合、クリアされます。

**Returns:**
byte - 時間フェーズデータのタイプ。
### getUid() {#getUid--}
```
public final int getUid()
```


時間フェーズデータの一意識別子を取得します

**Returns:**
int - 時間フェーズデータの一意識別子
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


時間フェーズデータ期間の時間単位を取得します。

**Returns:**
byte - 時間フェーズデータ期間の時間単位。
### getValue() {#getValue--}
```
public final String getValue()
```


時間フェーズデータ期間の時間単位あたりの値を取得します。

**Returns:**
java.lang.String - 時間フェーズデータ期間の単位時間あたりの値。
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


`double` インスタンスを取得します。このオブジェクトの文字列値を表します。

**Returns:**
double - オブジェクトの浮動小数点表現。
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


double インスタンスを取得します。このオブジェクトの文字列値を表します。

**Returns:**
double - オブジェクトの時間間隔表現。
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


`double` インスタンスを取得します。このオブジェクトの文字列値を、単位ベースの時間フェーズデータ用に表します。

**Returns:**
double - このオブジェクトの浮動小数点表現。
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


時間フェーズデータ期間の終了日を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 時間フェーズデータ期間の終了日。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


時間フェーズデータ期間の開始日を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 時間フェーズデータ期間の開始日。 |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


時間フェーズデータのタイプを設定します。

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) プロパティは、ここで指定された型に適さない場合、クリアされます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | バイト | 時間フェーズデータのタイプ。 |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


時間フェーズデータの一意識別子を設定します

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 時間フェーズデータの一意識別子。 |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


時間フェーズデータ期間の時間単位を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | バイト | 時間フェーズデータ期間の時間単位。 |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


時間フェーズデータ期間の時間単位あたりの値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 時間フェーズデータ期間の単位時間あたりの値。 |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


`double` インスタンスは、このオブジェクトの文字列値を表します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | `double` インスタンスは、このオブジェクトの文字列値を表します。 |

