---
title: "ビュー"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Project のビューを表します。"
type: docs
weight: 342
url: /ja/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Project のビューを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [View()](#View--) | 新しい [View](../../com.aspose.tasks/view) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | 現在のインスタンスを同じ型の別のオブジェクトと比較し、現在のインスタンスがソート順で前に来るか、後に来るか、または同じ位置にあるかを示す整数を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | 新しい [View](../../com.aspose.tasks/view) クラスのインスタンスを作成します。 |
| [getFilter()](#getFilter--) | 単一ビューで使用されるフィルターを取得します。 |
| [getGroup()](#getGroup--) | 単一ビューのグループを取得します。 |
| [getHighlightFilter()](#getHighlightFilter--) | Microsoft Project が単一ビューのフィルターをハイライト表示するかどうかを示す値を取得します。 |
| [getName()](#getName--) | View オブジェクトの名前を取得します。 |
| [getPageInfo()](#getPageInfo--) | `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) クラスのインスタンスを取得します。 |
| [getParentProject()](#getParentProject--) | View オブジェクトの親を取得します。 |
| [getScreen()](#getScreen--) | 単一ビューの画面タイプを取得します。 |
| [getShowInMenu()](#getShowInMenu--) | Microsoft Project がリボンの「ビュー」または「その他のビュー」ドロップダウンリストに単一ビュー名を表示するかどうかを示す値を取得します。 |
| [getTable()](#getTable--) | 単一ビューのテーブルを取得します。 |
| [getType()](#getType--) | タスクやリソースなど、単一ビュー内の項目のタイプを取得します。 |
| [getUid()](#getUid--) | ビューの一意識別子を取得します。 |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | ビュー内の [OleObject](../../com.aspose.tasks/oleobject) の配置と外観を表すオブジェクトのコレクションを取得します。 |
| [hashCode()](#hashCode--) | インスタンスの [Resource](../../com.aspose.tasks/resource) クラスのハッシュコード値を返します。 |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | このインスタンスが指定されたオブジェクトより大きいかどうかを示す値を返します。 |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | このインスタンスが指定されたオブジェクト以上かどうかを示す値を返します。 |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値を返します。 |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | このインスタンスが指定されたオブジェクトより小さいかどうかを示す値を返します。 |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | このインスタンスが指定されたオブジェクト以下かどうかを示す値を返します。 |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | 単一ビューで使用されるフィルターを設定します。 |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | 単一ビューのグループを設定します。 |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Microsoft Project が単一ビューのフィルターをハイライト表示するかどうかを示す値を設定します。 |
| [setName(String value)](#setName-java.lang.String-) | View オブジェクトの名前を設定します。 |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Microsoft Project がリボンの「ビュー」または「その他のビュー」ドロップダウンリストに単一ビュー名を表示するかどうかを示す値を設定します。 |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | 単一ビューのテーブルを設定します。 |
### View() {#View--}
```
public View()
```


新しい [View](../../com.aspose.tasks/view) クラスのインスタンスを初期化します。

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


現在のインスタンスを同じ型の別のオブジェクトと比較し、現在のインスタンスがソート順で前に来るか、後に来るか、または同じ位置にあるかを示す整数を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | このインスタンスと比較するための指定された View オブジェクトです。 |

**Returns:**
int - 比較対象のオブジェクトの相対順序を示す 32 ビット符号付き整数です。戻り値の意味は次のとおりです: 値の意味 0 未満 このインスタンスはソート順で `other` の前に来ます。 0 このインスタンスはソート順で `other` と同じ位置にあります。 0 より大きい このインスタンスはソート順で `other` の後に来ます。
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
boolean - 指定されたオブジェクトがこのインスタンスと同じ Uid 値を持つ View の場合は **True**、それ以外の場合は **false**です。
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


新しい [View](../../com.aspose.tasks/view) クラスのインスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| viewScreen | int | ビューを表示できる画面タイプです。 |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


単一ビューで使用されるフィルターを取得します。

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


単一ビューのグループを取得します。

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Microsoft Project が単一ビューのフィルターをハイライト表示するかどうかを示す値を取得します。

**Returns:**
boolean - Microsoft Project が単一ビューのフィルターをハイライトするかどうかを示す値です。
### getName() {#getName--}
```
public final String getName()
```


View オブジェクトの名前を取得します。

**Returns:**
java.lang.String - View オブジェクトの名前です。
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


`PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) クラスのインスタンスを取得します。mpp ファイル形式に存在するページ設定データを表します。

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


View オブジェクトの親を取得します。読み取り専用 [Project](../../com.aspose.tasks/project)。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


単一ビューの画面タイプを取得します。読み取り専用 [ViewScreen](../../com.aspose.tasks/viewscreen)。

**Returns:**
int - 単一ビューの画面タイプです。
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Microsoft Project がリボンの「ビュー」または「その他のビュー」ドロップダウンリストに単一ビュー名を表示するかどうかを示す値を取得します。

**Returns:**
boolean - Microsoft Project がリボンの View または Other Views ドロップダウンリストに単一ビュー名を表示するかどうかを示す値です。
### getTable() {#getTable--}
```
public final Table getTable()
```


単一ビューのテーブルを取得します。

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


単一ビュー内の項目の種類（タスクやリソースなど）を取得します。読み取り専用 [ItemType](../../com.aspose.tasks/itemtype)。

**Returns:**
int - 単一ビュー内の項目の種類（タスクやリソースなど）です。
### getUid() {#getUid--}
```
public final int getUid()
```


ビューの一意識別子を取得します。

**Returns:**
int - ビューの一意識別子です。
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


ビュー内の [OleObject](../../com.aspose.tasks/oleobject) の配置と外観を表すオブジェクトのコレクションを取得します。

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - ビュー内の [OleObject](../../com.aspose.tasks/oleobject) の配置と外観を表すオブジェクトのコレクションです。
### hashCode() {#hashCode--}
```
public int hashCode()
```


インスタンスの [Resource](../../com.aspose.tasks/resource) クラスのハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 最初のビューです。 |
| b | [View](../../com.aspose.tasks/view) | 2 番目のビューです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しいかどうかを示す値
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


このインスタンスが指定されたオブジェクトより大きいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 最初のビューです。 |
| b | [View](../../com.aspose.tasks/view) | 2 番目のビューです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトより大きいかどうかを示す値
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


このインスタンスが指定されたオブジェクト以上かどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 最初のビューです。 |
| b | [View](../../com.aspose.tasks/view) | 2 番目のビューです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクト以上かどうかを示す値
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 最初のビューです。 |
| b | [View](../../com.aspose.tasks/view) | 2 番目のビューです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しくないかどうかを示す値
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


このインスタンスが指定されたオブジェクトより小さいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 最初のフィルター。 |
| b | [View](../../com.aspose.tasks/view) | 2番目のフィルター。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトより小さいかどうかを示す値
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


このインスタンスが指定されたオブジェクト以下かどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 最初のビューです。 |
| b | [View](../../com.aspose.tasks/view) | 2 番目のビューです。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクト以下かどうかを示す値
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


単一ビューで使用されるフィルターを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | 単一ビューで使用されるフィルターです。 |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


単一ビューのグループを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | 単一ビューのグループです。 |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Microsoft Project が単一ビューのフィルターをハイライト表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | Microsoft Project が単一ビューのフィルターをハイライトするかどうかを示す値です。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


View オブジェクトの名前を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | View オブジェクトの名前です。 |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Microsoft Project がリボンの「ビュー」または「その他のビュー」ドロップダウンリストに単一ビュー名を表示するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | Microsoft Project がリボンの View または Other Views ドロップダウンリストに単一ビュー名を表示するかどうかを示す値です。 |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


単一ビューのテーブルを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | 単一ビューのテーブルです。 |

