---
title: "ViewCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのリストを含みます。"
type: docs
weight: 343
url: /ja/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

[View](../../com.aspose.tasks/view) オブジェクトのリストを含みます。`AbstractCollection` クラスを継承しています。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | 指定された項目をこのコレクションに追加します。 |
| [clear()](#clear--) | このコレクションからすべての項目を削除します。 |
| [contains(View item)](#contains-com.aspose.tasks.View-) | 指定された項目がこのコレクションに見つかった場合は true を返し、そうでない場合は false を返します。 |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | このコレクションの要素を、指定された配列インデックスから開始して、指定された配列にコピーします。 |
| [getByName(String viewName)](#getByName-java.lang.String-) | 名前で View を検索し、コレクション内で最初に見つかったものを返します。 |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | 指定された Screen プロパティを持つ View を検索し、コレクション内で最初に見つかったものを返します。 |
| [getParentProject()](#getParentProject--) | View オブジェクトの親を取得します。 |
| [iterator()](#iterator--) | このコレクションに含まれる要素のイテレータを返します。 |
| [remove(View item)](#remove-com.aspose.tasks.View-) | このコレクションから特定のオブジェクトの最初の出現を削除します。 |
| [size()](#size--) | このコレクションに含まれる要素数を取得します。 |
| [toList()](#toList--) | ビューコレクションを [View](../../com.aspose.tasks/view) オブジェクトのリストに変換します。 |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


指定された項目をこのコレクションに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | このコレクションに追加する指定された項目。 |

**Returns:**
boolean - 操作が成功した場合は true。
### clear() {#clear--}
```
public final void clear()
```


このコレクションからすべての項目を削除します。

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


指定された項目がこのコレクションに見つかった場合は true を返し、そうでない場合は false を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | 検索する指定された項目。 |

**Returns:**
boolean - 指定された項目がこのコレクションに見つかった場合は true、そうでない場合は false。
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


このコレクションの要素を、指定された配列インデックスから開始して、指定された配列にコピーします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | 要素をコピーする先の指定された一次元配列 |
| arrayIndex | int | コピーが開始される指定された配列のゼロベースインデックス。 |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


名前で View を検索し、コレクション内で最初に見つかったものを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| viewName | java.lang.String | 検索対象の View の名前。 |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


指定された Screen プロパティを持つ View を検索し、コレクション内で最初に見つかったものを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| screen | int | [ViewScreen](../../com.aspose.tasks/viewscreen) 列挙値。 |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


View オブジェクトの親を取得します。読み取り専用 [Project](../../com.aspose.tasks/project)。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


このコレクションに含まれる要素のイテレータを返します。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - コレクションイテレータ。
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


このコレクションから特定のオブジェクトの最初の出現を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | 削除する指定されたオブジェクト。 |

**Returns:**
boolean - 指定されたオブジェクトがこのコレクションから正常に削除された場合は true、そうでない場合は false。
### size() {#size--}
```
public final int size()
```


このコレクションに含まれる要素数を取得します。

**Returns:**
int - このコレクションに含まれる要素数。
### toList() {#toList--}
```
public final List<View> toList()
```


ビューコレクションを [View](../../com.aspose.tasks/view) オブジェクトのリストに変換します。

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - [View](../../com.aspose.tasks/view) オブジェクトの汎用リスト。
