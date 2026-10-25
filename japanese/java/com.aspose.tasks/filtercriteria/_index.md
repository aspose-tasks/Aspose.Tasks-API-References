---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "MSP ビューに表示されるためにタスクまたはリソースが満たすべき基準を定義します。"
type: docs
weight: 94
url: /ja/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

MSP ビューに表示されるためにタスクまたはリソースが満たすべき基準を定義します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | 子[FilterCriteria](../../com.aspose.tasks/filtercriteria)行のリストを取得します。 |
| [getField()](#getField--) | 変更するための`Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))を取得します。 |
| [getOperation()](#getOperation--) | FieldName、Test、Valueで設定された基準がフィルタ内の他の基準と関連するかを取得します。 |
| [getTest()](#getTest--) | フィルタの選択基準として機能する、FieldNameとValue間の比較タイプを取得します。 |
| [getValues()](#getValues--) | FieldNameで指定されたフィールドの値と比較するオブジェクト値を取得します。 |
| [isValueAField()](#isValueAField--) | FilterCriteriaの右側の値が定数ではなくフィールド参照であるかどうかを取得します。 |
| [isValueAField(int index)](#isValueAField-int-) | FilterCriteriaのインデックス位置の値が定数ではなくフィールド参照であるかどうかを取得します。 |
| [setField(int value)](#setField-int-) | 変更するために`Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))を設定します。 |
| [setOperation(int value)](#setOperation-int-) | フィルタ内の他の基準と関連する、FieldName、Test、Valueで設定された基準を設定します。 |
| [setTest(int value)](#setTest-int-) | フィルタの選択基準として機能する、FieldName と Value の間で行われる比較のタイプを設定します。 |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | FieldName で指定されたフィールドの値と比較するために、インデックス位置のオブジェクト値を設定します。 |
| [setValue(Object value)](#setValue-java.lang.Object-) | FieldName で指定されたフィールドの値と比較するオブジェクト値を設定します。 |
| [setValueByField(int value)](#setValueByField-int-) | FieldName で指定されたフィールドの値と比較されるフィールドを設定します。 |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | FieldName で指定されたフィールドの値と比較される、インデックス位置のフィールドを設定します。 |
| [toString()](#toString--) | [FilterCriteria](../../com.aspose.tasks/filtercriteria) クラスのインスタンスの文字列表現を返します。 |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


子 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 行のリストを取得します。フィルタに複数の基準行が含まれる場合、And 演算子の効果は、両方の行の基準が満たされることがタスクまたはリソースがこのフィルタの結果として表示される条件となります。Or 演算子の効果は、いずれか一方の行の基準が満たされることです。

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - 子 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 行のリストです。
### getField() {#getField--}
```
public final int getField()
```


変更するための`Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))を取得します。

**Returns:**
int - 変更する `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))。
### getOperation() {#getOperation--}
```
public final int getOperation()
```


FieldName、Test、Valueで設定された基準がフィルタ内の他の基準と関連するかを取得します。

**Returns:**
int - FieldName、Test、Valueで設定された基準がフィルタ内の他の基準と関連します。
### getTest() {#getTest--}
```
public final int getTest()
```


FieldName と Value の間で行われる比較のタイプを取得します。これはフィルタの選択基準として機能します。 [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - FieldName と Value の間で行われる比較のタイプで、フィルタの選択基準として機能します。
### getValues() {#getValues--}
```
public final Object[] getValues()
```


FieldNameで指定されたフィールドの値と比較するオブジェクト値を取得します。

**Returns:**
java.lang.Object[] - FieldName で指定されたフィールドの値と比較するオブジェクト値です。
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


FilterCriteriaの右側の値が定数ではなくフィールド参照であるかどうかを取得します。

**Returns:**
boolean - FilterCriteria の右側の値が定数値ではなくフィールド参照であるかどうかを示します。
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


FilterCriteriaのインデックス位置の値が定数ではなくフィールド参照であるかどうかを取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 値のインデックス |

**Returns:**
boolean - FilterCriteria のインデックス位置の右側の値が定数値ではなくフィールド参照であるかどうかを示します。
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


変更するために`Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) を変更します。 |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


フィルタ内の他の基準と関連する、FieldName、Test、Valueで設定された基準を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | FieldName、Test、Valueで設定された基準がフィルタ内の他の基準と関連します。 |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


FieldName と Value の間で行われる比較のタイプを設定します。これはフィルタの選択基準として機能します。 [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | FieldName と Value の間で行われる比較のタイプで、フィルタの選択基準として機能します。 |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


FieldName で指定されたフィールドの値と比較するために、インデックス位置のオブジェクト値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 値のインデックスです。 |
| 値 | java.lang.Object | フィルタ基準のインデックス位置で右側の値として使用されるオブジェクト値です。 |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


FieldName で指定されたフィールドの値と比較するオブジェクト値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.Object | フィルタ基準の右側の値として使用されるオブジェクト値です。 |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


FieldName で指定されたフィールドの値と比較されるフィールドを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | フィルタ基準の右側の値として使用されるフィールドです。 |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


FieldName で指定されたフィールドの値と比較される、インデックス位置のフィールドを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 値のインデックス |
| 値 | int | フィルタ条件のインデックスで右側の値として使用されるフィールド。 |

### toString() {#toString--}
```
public String toString()
```


[FilterCriteria](../../com.aspose.tasks/filtercriteria) クラスのインスタンスの文字列表現を返します。

**Returns:**
java.lang.String - このオブジェクトの文字列表現。
