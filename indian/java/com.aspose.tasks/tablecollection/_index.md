---
title: "TableCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स की एक सूची शामिल करता है।"
type: docs
weight: 285
url: /hi/java/com.aspose.tasks/tablecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class TableCollection extends AbstractCollection<Table>
```

ऑब्जेक्ट्स की एक सूची शामिल करता है जिसमें [Table](../../com.aspose.tasks/table) शामिल हैं। ICollection&lt;Table&gt; इंटरफ़ेस को लागू करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(Table item)](#add-com.aspose.tasks.Table-) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [clear()](#clear--) | इस संग्रह से सभी आइटम हटाता है। |
| [contains(Table item)](#contains-com.aspose.tasks.Table-) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [copyTo(Table[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Table---int-) | इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है, निर्दिष्ट एरे इंडेक्स से शुरू होकर। |
| [iterator()](#iterator--) | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [remove(Table item)](#remove-com.aspose.tasks.Table-) | इस संग्रह से किसी विशिष्ट ऑब्जेक्ट की पहली उपस्थिति हटाता है। |
| [size()](#size--) | इस संग्रह में शामिल तत्वों की संख्या प्राप्त करता है। |
| [toList()](#toList--) | एक टेबल संग्रह को [Table](../../com.aspose.tasks/table) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |
### add(Table item) {#add-com.aspose.tasks.Table-}
```
public final boolean add(Table item)
```


निर्दिष्ट आइटम को इस संग्रह में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [Table](../../com.aspose.tasks/table) | इस संग्रह में जोड़ने के लिए निर्दिष्ट आइटम। |

**Returns:**
बूलियन - यदि जोड़ने का ऑपरेशन सफल रहा और आइटम संग्रह में जोड़ा गया हो तो true।
### clear() {#clear--}
```
public final void clear()
```


इस संग्रह से सभी आइटम हटाता है।

### contains(Table item) {#contains-com.aspose.tasks.Table-}
```
public final boolean contains(Table item)
```


यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [Table](../../com.aspose.tasks/table) | खोजने के लिए निर्दिष्ट आइटम। |

**Returns:**
बूलियन - यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true; अन्यथा false।
### copyTo(Table[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Table---int-}
```
public final void copyTo(Table[] array, int arrayIndex)
```


इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है, निर्दिष्ट एरे इंडेक्स से शुरू होकर।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| array | [Table\[\]](../../com.aspose.tasks/table) | तत्वों को कॉपी करने के लिए निर्दिष्ट एक-आयामी एरे। |
| arrayIndex | int | निर्दिष्ट एरे का शून्य-आधारित सूचकांक जहाँ प्रतिलिपि शुरू होती है। |

### iterator() {#iterator--}
```
public final Iterator<Table> iterator()
```


इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Table&gt; - इस संग्रह के लिए एक इटरेटर।
### remove(Table item) {#remove-com.aspose.tasks.Table-}
```
public final boolean remove(Table item)
```


इस संग्रह से किसी विशिष्ट ऑब्जेक्ट की पहली उपस्थिति हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [Table](../../com.aspose.tasks/table) | हटाने के लिए निर्दिष्ट वस्तु। |

**Returns:**
boolean - true यदि निर्दिष्ट वस्तु को इस संग्रह से सफलतापूर्वक हटा दिया गया हो; अन्यथा false।
### size() {#size--}
```
public final int size()
```


इस संग्रह में शामिल तत्वों की संख्या प्राप्त करता है।

**Returns:**
int - इस संग्रह में शामिल तत्वों की संख्या।
### toList() {#toList--}
```
public final List<Table> toList()
```


एक टेबल संग्रह को [Table](../../com.aspose.tasks/table) ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.Table&gt; - [Table](../../com.aspose.tasks/table) वस्तुओं की सामान्य सूची।
