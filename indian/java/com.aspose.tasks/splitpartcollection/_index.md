---
title: "SplitPartCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक संग्रह जो कार्य के भागों का प्रतिनिधित्व करता है।"
type: docs
weight: 279
url: /hi/java/com.aspose.tasks/splitpartcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class SplitPartCollection extends AbstractList<SplitPart>
```

एक संग्रह जो कार्य के भागों का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [get(int index)](#get-int-) | दिए गए इंडेक्स पर टास्क का स्प्लिट पार्ट प्राप्त करता है। |
| [set(int index, SplitPart value)](#set-int-com.aspose.tasks.SplitPart-) | दिए गए इंडेक्स पर टास्क का स्प्लिट पार्ट सेट करता है। |
| [size()](#size--) | संग्रह में भागों की संख्या प्राप्त करता है। |
| [toArray()](#toArray--) | संग्रह से सभी भागों को नई एरे में कॉपी करता है। |
### get(int index) {#get-int-}
```
public final SplitPart get(int index)
```


दिए गए इंडेक्स पर टास्क का स्प्लिट पार्ट प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | सूचकांक | int | भाग का इंडेक्स। |

--------------------

इंडेक्स शून्य-आधारित है। यदि इंडेक्स एरे की सीमाओं के बाहर है तो null लौटाता है। |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### set(int index, SplitPart value) {#set-int-com.aspose.tasks.SplitPart-}
```
public final SplitPart set(int index, SplitPart value)
```


दिए गए इंडेक्स पर टास्क का स्प्लिट पार्ट सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | सूचकांक | int | भाग का इंडेक्स। |

--------------------

इंडेक्स शून्य-आधारित है। यदि इंडेक्स एरे की सीमाओं के बाहर है तो null लौटाता है। |
| value | [SplitPart](../../com.aspose.tasks/splitpart) | सेट करने के लिए एक स्प्लिट पार्ट। |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### size() {#size--}
```
public final int size()
```


संग्रह में भागों की संख्या प्राप्त करता है।

**Returns:**
int - संग्रह में भागों की संख्या।
### toArray() {#toArray--}
```
public final SplitPart[] toArray()
```


संग्रह से सभी भागों को नई एरे में कॉपी करता है।

**Returns:**
com.aspose.tasks.SplitPart[] - [SplitPart](../../com.aspose.tasks/splitpart) ऑब्जेक्ट्स की एक एरे।
