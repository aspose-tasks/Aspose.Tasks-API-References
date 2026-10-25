---
title: "OleObjectCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示一个包含该类实例的集合。"
type: docs
weight: 165
url: /zh/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

表示一个包含 [OleObject](../../com.aspose.tasks/oleobject) 类实例的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | 清除集合。 |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | 返回此集合中的元素数量。 |
| [toList()](#toList--) | 将 [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) 类的实例转换为包含 [OleObject](../../com.aspose.tasks/oleobject) 类实例的列表。 |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


清除集合。为了持久化这些更改，应使用 new MPPSaveOptions \{ WriteViewData = true; \} 调用 project.Save。

--------------------

&gt; ```
&gt; 如何清除 OLE 对象并持久化这些更改。
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
