---
title: "OleObjectCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "クラスのインスタンスを含むコレクションを表します。"
type: docs
weight: 165
url: /ja/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

[OleObject](../../com.aspose.tasks/oleobject) クラスのインスタンスを含むコレクションを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | コレクションをクリアします。 |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | このコレクションの要素数を返します。 |
| [toList()](#toList--) | [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) クラスのインスタンスを、[OleObject](../../com.aspose.tasks/oleobject) クラスのインスタンスを含むリストに変換します。 |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


コレクションをクリアします。これらの変更を永続化するには、new MPPSaveOptions \{ WriteViewData = true; \} を使用して project.Save を呼び出す必要があります。

--------------------

&gt; ```
&gt; OLE オブジェクトをクリアし、これらの変更を永続化する方法。
&gt; ``````

 [C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
 
```



### get(int index) {#get-int-}
```
public OleObject get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[OleObject](../../com.aspose.tasks/oleobject) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


Returns the number of elements in this collection.

**Returns:**
int - the number of elements in this collection.
### toList() {#toList--}
```
public final List<OleObject> toList()
```


Converts the instance of the [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) class to a list containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class.

**Returns:**
java.util.List&lt;com.aspose.tasks.OleObject&gt; - Converted to list the instance of the [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) class containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class.
