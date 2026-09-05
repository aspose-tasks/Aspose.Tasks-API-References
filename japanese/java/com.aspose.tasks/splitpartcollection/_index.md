---
title: "SplitPartCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "タスクの各部分を表すコレクションです。"
type: docs
weight: 279
url: /ja/java/com.aspose.tasks/splitpartcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class SplitPartCollection extends AbstractList<SplitPart>
```

タスクの各部分を表すコレクションです。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [get(int index)](#get-int-) | 指定されたインデックスのタスクの分割パートを取得します。 |
| [set(int index, SplitPart value)](#set-int-com.aspose.tasks.SplitPart-) | 指定されたインデックスのタスクの分割パートを設定します。 |
| [size()](#size--) | コレクション内のパート数を取得します。 |
| [toArray()](#toArray--) | コレクションからすべてのパートを新しい配列にコピーします。 |
### get(int index) {#get-int-}
```
public final SplitPart get(int index)
```


指定されたインデックスのタスクの分割パートを取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | インデックス | int | パートのインデックスです。 |

--------------------

インデックスはゼロベースです。インデックスが配列の範囲外の場合は null を返します。 |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### set(int index, SplitPart value) {#set-int-com.aspose.tasks.SplitPart-}
```
public final SplitPart set(int index, SplitPart value)
```


指定されたインデックスのタスクの分割パートを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | インデックス | int | パートのインデックスです。 |

--------------------

インデックスはゼロベースです。インデックスが配列の範囲外の場合は null を返します。 |
| value | [SplitPart](../../com.aspose.tasks/splitpart) | 設定する分割パートです。 |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### size() {#size--}
```
public final int size()
```


コレクション内のパート数を取得します。

**Returns:**
int - コレクション内のパーツの数。
### toArray() {#toArray--}
```
public final SplitPart[] toArray()
```


コレクションからすべてのパートを新しい配列にコピーします。

**Returns:**
com.aspose.tasks.SplitPart[] - [SplitPart](../../com.aspose.tasks/splitpart) オブジェクトの配列。
