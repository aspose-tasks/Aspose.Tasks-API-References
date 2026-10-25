---
title: "OleObjectCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "인스턴스를 포함하는 컬렉션을 나타냅니다."
type: docs
weight: 165
url: /ko/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

[OleObject](../../com.aspose.tasks/oleobject) 클래스의 인스턴스를 포함하는 컬렉션을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | 컬렉션을 비웁니다. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | 이 컬렉션의 요소 수를 반환합니다. |
| [toList()](#toList--) | [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) 클래스의 인스턴스를 [OleObject](../../com.aspose.tasks/oleobject) 클래스의 인스턴스를 포함하는 리스트로 변환합니다. |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


컬렉션을 비웁니다. 이러한 변경 사항을 지속하려면 project.Save를 새 MPPSaveOptions \{ WriteViewData = true; \}와 함께 호출해야 합니다.

--------------------

&gt; ```
&gt; OLE 객체를 지우고 이러한 변경 사항을 지속하는 방법.
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
