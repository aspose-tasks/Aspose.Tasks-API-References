---
title: "ベースライン"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "リソースのベースライン値を表します。"
type: docs
weight: 26
url: /ja/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

リソースのベースライン値を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | IComparable インターフェイスの実装。 |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getBaselineNumber()](#getBaselineNumber--) | ベースライン データ レコードの一意の番号を取得します。 |
| [getBcwp()](#getBcwp--) | リソースがプロジェクトで実施した作業の予算コスト（現在まで）を取得します。 |
| [getBcws()](#getBcws--) | リソースに予定された作業の予算コストを取得します。 |
| [getCost()](#getCost--) | ベースラインが保存されたときのリソースの予測コストを取得します。 |
| [getWork()](#getWork--) | ベースラインが保存されたときにリソースに割り当てられた作業を取得します。 |
| [hashCode()](#hashCode--) | ベースラインのハッシュコード値を返します。 |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | このインスタンスが指定されたオブジェクトより大きいかどうかを示す値を返します。 |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | このインスタンスが指定されたオブジェクト以上かどうかを示す値を返します。 |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値を返します。 |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | このインスタンスが指定されたオブジェクトより小さいかどうかを示す値を返します。 |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | このインスタンスが指定されたオブジェクト以下かどうかを示す値を返します。 |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | ベースライン データ レコードの一意の番号を設定します。 |
| [setBcwp(double value)](#setBcwp-double-) | リソースがプロジェクトで実施した作業の予算コスト（現在まで）を設定します。 |
| [setBcws(double value)](#setBcws-double-) | リソースに予定された作業の予算コストを設定します。 |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | ベースラインが保存されたときのリソースの予測コストを設定します。 |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | ベースラインが保存されたときにリソースに割り当てられた作業を設定します。 |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


IComparable インターフェイスの実装です。このインスタンスを指定された Baseline オブジェクトと比較します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | このインスタンスと比較するための指定された Baseline オブジェクト。 |

**Returns:**
int - このインスタンスが指定されたオブジェクトより小さい場合は -1、指定されたオブジェクトより大きい場合は 1 を返し、それ以外の場合は 0 を返します。
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | このインスタンスと比較するための指定されたオブジェクト。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しい場合は true を返し、そうでない場合は false を返します。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するための指定されたオブジェクト。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しい場合は true を返し、そうでない場合は false を返します。
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


ベースライン データ レコードの一意の番号を取得します。

**Returns:**
int - ベースラインデータレコードの一意の番号です。
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


リソースがプロジェクトで実施した作業の予算コスト（現在まで）を取得します。

**Returns:**
double - リソースがプロジェクトのために実施した作業の予算コスト（現在まで）です。
### getBcws() {#getBcws--}
```
public final double getBcws()
```


リソースに予定された作業の予算コストを取得します。

**Returns:**
double - リソースに予定された作業の予算コストです。
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


ベースラインが保存されたときのリソースの予測コストを取得します。

**Returns:**
java.math.BigDecimal - ベースラインが保存されたときのリソースの予測コストです。
### getWork() {#getWork--}
```
public final Duration getWork()
```


ベースラインが保存されたときにリソースに割り当てられた作業を取得します。

値: ベースラインが保存されたときにリソースに割り当てられた作業量です。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


ベースラインのハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 最初のベースラインです。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 2番目のベースラインです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しいかどうかを示す値
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


このインスタンスが指定されたオブジェクトより大きいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 最初のベースラインです。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 2番目のベースラインです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトより大きいかどうかを示す値
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


このインスタンスが指定されたオブジェクト以上かどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 最初のベースラインです。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 2番目のベースラインです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクト以上かどうかを示す値
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 最初のベースラインです。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 2番目のベースラインです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


このインスタンスが指定されたオブジェクトより小さいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 最初のベースラインです。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 2番目のベースラインです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトより小さいかどうかを示す値
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


このインスタンスが指定されたオブジェクト以下かどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 最初のベースラインです。 |
| b | [Baseline](../../com.aspose.tasks/baseline) | 2番目のベースラインです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクト以下かどうかを示す値
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


ベースライン データ レコードの一意の番号を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | ベースラインデータレコードの一意の番号です。 |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


リソースがプロジェクトで実施した作業の予算コスト（現在まで）を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | リソースがプロジェクトのために実施した作業の予算コスト（現在まで）です。 |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


リソースに予定された作業の予算コストを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | リソースに予定された作業の予算コストです。 |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


ベースラインが保存されたときのリソースの予測コストを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.math.BigDecimal | ベースラインが保存されたときのリソースの予測コストです。 |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


ベースラインが保存されたときにリソースに割り当てられた作業を設定します。

値: ベースラインが保存されたときにリソースに割り当てられた作業量です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ベースラインが保存されたときにリソースに割り当てられた作業です。 |

