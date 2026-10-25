---
title: "OleObjectCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "क्लास की इंस्टेंस को सम्मिलित करने वाला संग्रह दर्शाता है।"
type: docs
weight: 165
url: /hi/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

क्लास की इंस्टेंस को सम्मिलित करने वाला संग्रह दर्शाता है जिसमें [OleObject](../../com.aspose/tasks/oleobject) क्लास शामिल है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | संग्रह को साफ़ करता है। |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | इस संग्रह में तत्वों की संख्या लौटाता है। |
| [toList()](#toList--) | यह [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) क्लास की इंस्टेंस को एक सूची में बदलता है जिसमें [OleObject](../../com.aspose.tasks/oleobject) क्लास की इंस्टेंस शामिल हैं। |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


संग्रह को साफ़ करता है। इन परिवर्तनों को स्थायी बनाने के लिए project.Save को नए MPPSaveOptions \{ WriteViewData = true; \} के साथ कॉल किया जाना चाहिए।

--------------------

&gt; ```
&gt; OLE ऑब्जेक्ट्स को साफ़ करने और इन परिवर्तनों को स्थायी बनाने का तरीका।
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
