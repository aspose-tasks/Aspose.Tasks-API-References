---
title: "フィルター"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Project のフィルターを表します。"
type: docs
weight: 91
url: /ja/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Project のフィルターを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [Filter()](#Filter--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | このインスタンスを [Filter](../../com.aspose.tasks/filter) クラスの指定されたインスタンスと比較し、相対的な順序を示す指標を返します。 |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | このインスタンスが指定された AssignmentBaseline オブジェクトと等しいかどうかを示す値を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定された AssignmentBaseline オブジェクトと等しいかどうかを示す値を返します。 |
| [getCriteria()](#getCriteria--) | MSP ビューに表示されるためにタスクまたはリソースが満たす必要がある基準を取得します。 |
| [getFilterType()](#getFilterType--) | フィルターのタイプを取得します。 |
| [getIndex()](#getIndex--) | Filters を含むオブジェクト内の [Filter](../../com.aspose.tasks/filter) オブジェクトのインデックスを取得します。 |
| [getName()](#getName--) | Filter オブジェクトの名前を取得します。 |
| [getShowInMenu()](#getShowInMenu--) | リボンの View タブの Filter ドロップダウンリストにプロジェクトがフィルタ名を表示するかどうかを示す値を取得します。 |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | フィルタに対して関連するサマリ行が表示されるかどうかを示す値を取得します。 |
| [getUid()](#getUid--) | フィルタの一意の識別子を取得します。 |
| [hashCode()](#hashCode--) | フィルタのハッシュコード値を返します。 |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | このインスタンスが指定されたオブジェクトより大きいかどうかを示す値を返します。 |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | このインスタンスが指定されたオブジェクト以上かどうかを示す値を返します。 |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値を返します。 |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | このインスタンスが指定されたオブジェクトより小さいかどうかを示す値を返します。 |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | このインスタンスが指定されたオブジェクト以下かどうかを示す値を返します。 |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | MSP ビューに表示されるためにタスクまたはリソースが満たす必要がある基準を設定します。 |
| [setFilterType(int value)](#setFilterType-int-) | フィルタのタイプです。 |
| [setName(String value)](#setName-java.lang.String-) | Filter オブジェクトの名前を設定します。 |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | リボンの View タブの Filter ドロップダウンリストにプロジェクトがフィルタ名を表示するかどうかを示す値を設定します。 |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | フィルタに対して関連するサマリ行が表示されるかどうかを示す値を設定します。 |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


このインスタンスを [Filter](../../com.aspose.tasks/filter) クラスの指定されたインスタンスと比較し、相対的な順序を示す指標を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | このオブジェクトと比較するための指定された [Filter](../../com.aspose.tasks/filter) クラスのインスタンスです。 |

**Returns:**
int - 相対的な順序を示す指標です。
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


このインスタンスが指定された AssignmentBaseline オブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | このインスタンスと比較するための指定された AssignmentBaseline オブジェクトです。 |

**Returns:**
boolean - このインスタンスが指定された AssignmentBaseline オブジェクトと等しい場合は true を返し、そうでない場合は false を返します。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定された AssignmentBaseline オブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するための指定された AssignmentBaseline オブジェクトです。 |

**Returns:**
boolean - このインスタンスが指定された AssignmentBaseline オブジェクトと等しい場合は true を返し、そうでない場合は false を返します。
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


MSP ビューに表示されるためにタスクまたはリソースが満たす必要がある基準を取得します。

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


フィルターのタイプを取得します。

**Returns:**
int - フィルタのタイプです。
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Filters を含むオブジェクト内の [Filter](../../com.aspose.tasks/filter) オブジェクトのインデックスを取得します。

**Returns:**
int - Filters を含むオブジェクト内の [Filter](../../com.aspose.tasks/filter) オブジェクトのインデックスです。
### getName() {#getName--}
```
public final String getName()
```


Filter オブジェクトの名前を取得します。

**Returns:**
java.lang.String - Filter オブジェクトの名前です。
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


リボンの View タブの Filter ドロップダウンリストにプロジェクトがフィルタ名を表示するかどうかを示す値を取得します。

**Returns:**
boolean - プロジェクトがリボンの表示タブのフィルター ドロップダウン リストにフィルター名を表示するかどうかを示す値。
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


フィルタに対して関連するサマリ行が表示されるかどうかを示す値を取得します。

**Returns:**
boolean - フィルターに対して関連するサマリ行が表示されるかどうかを示す値。
### getUid() {#getUid--}
```
public final int getUid()
```


フィルタの一意の識別子を取得します。

**Returns:**
int - フィルターの一意の識別子。
### hashCode() {#hashCode--}
```
public int hashCode()
```


フィルタのハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 最初のフィルター。 |
| b | [Filter](../../com.aspose.tasks/filter) | 2番目のフィルター。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しいかどうかを示す値
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


このインスタンスが指定されたオブジェクトより大きいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 最初のフィルター。 |
| b | [Filter](../../com.aspose.tasks/filter) | 2番目のフィルター。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトより大きいかどうかを示す値
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


このインスタンスが指定されたオブジェクト以上かどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 最初のフィルター。 |
| b | [Filter](../../com.aspose.tasks/filter) | 2番目のフィルター。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクト以上かどうかを示す値
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 最初のフィルター。 |
| b | [Filter](../../com.aspose.tasks/filter) | 2番目のフィルター。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


このインスタンスが指定されたオブジェクトより小さいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 最初のフィルター。 |
| b | [Filter](../../com.aspose.tasks/filter) | 2番目のフィルター。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトより小さいかどうかを示す値
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


このインスタンスが指定されたオブジェクト以下かどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 最初のフィルター。 |
| b | [Filter](../../com.aspose.tasks/filter) | 2番目のフィルター。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクト以下かどうかを示す値
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


MSP ビューに表示されるためにタスクまたはリソースが満たす必要がある基準を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | MSP ビューに表示されるためにタスクまたはリソースが満たす必要がある基準。 |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


フィルタのタイプです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | フィルターのタイプ。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Filter オブジェクトの名前を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Filter オブジェクトの名前。 |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


リボンの View タブの Filter ドロップダウンリストにプロジェクトがフィルタ名を表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトがリボンの表示タブのフィルター ドロップダウン リストにフィルター名を表示するかどうかを示す値。 |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


フィルタに対して関連するサマリ行が表示されるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | フィルターに対して関連するサマリ行が表示されるかどうかを示す値。 |

