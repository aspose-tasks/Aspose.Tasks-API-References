---
title: "ViewCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स की एक सूची शामिल करता है।"
type: docs
weight: 343
url: /hi/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

[View](../../com.aspose.tasks/view) ऑब्जेक्ट्स की एक सूची शामिल है। `AbstractCollection` क्लास को विस्तारित करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [clear()](#clear--) | इस संग्रह से सभी आइटम हटाता है। |
| [contains(View item)](#contains-com.aspose.tasks.View-) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है, निर्दिष्ट एरे इंडेक्स से शुरू होकर। |
| [getByName(String viewName)](#getByName-java.lang.String-) | नाम के साथ एक View की खोज करता है, और संग्रह में पहली घटना लौटाता है। |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | निर्दिष्ट Screen प्रॉपर्टी वाले View की खोज करता है, और संग्रह में पहली घटना लौटाता है। |
| [getParentProject()](#getParentProject--) | View वस्तु का पैरेंट प्राप्त करता है। |
| [iterator()](#iterator--) | इस संग्रह में मौजूद तत्वों पर एक इटररेटर लौटाता है। |
| [remove(View item)](#remove-com.aspose.tasks.View-) | इस संग्रह से किसी विशिष्ट ऑब्जेक्ट की पहली उपस्थिति हटाता है। |
| [size()](#size--) | इस संग्रह में शामिल तत्वों की संख्या प्राप्त करता है। |
| [toList()](#toList--) | एक view संग्रह को [View](../../com.aspose.tasks/view) ऑब्जेक्ट्स की सूची में बदलता है। |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


निर्दिष्ट आइटम को इस संग्रह में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | इस संग्रह में जोड़ने के लिए निर्दिष्ट आइटम। |

**Returns:**
boolean - यदि ऑपरेशन सफल रहा तो true।
### clear() {#clear--}
```
public final void clear()
```


इस संग्रह से सभी आइटम हटाता है।

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | खोजने के लिए निर्दिष्ट आइटम। |

**Returns:**
बूलियन - यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true; अन्यथा false।
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है, निर्दिष्ट एरे इंडेक्स से शुरू होकर।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | तत्वों को कॉपी करने के लिए निर्दिष्ट एक-आयामी एरे। |
| arrayIndex | int | निर्दिष्ट एरे का शून्य-आधारित सूचकांक जहाँ प्रतिलिपि शुरू होती है। |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


नाम के साथ एक View की खोज करता है, और संग्रह में पहली घटना लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| viewName | java.lang.String | खोजने के लिए View का नाम। |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


निर्दिष्ट Screen प्रॉपर्टी वाले View की खोज करता है, और संग्रह में पहली घटना लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| screen | int | [ViewScreen](../../com.aspose.tasks/viewscreen) एन्यूमरेशन मान। |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


View ऑब्जेक्ट का पैरेंट प्राप्त करता है। केवल‑पढ़ने योग्य [Project](../../com.aspose.tasks/project)।

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


इस संग्रह में मौजूद तत्वों पर एक इटररेटर लौटाता है।

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - संग्रह इटररेटर।
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


इस संग्रह से किसी विशिष्ट ऑब्जेक्ट की पहली उपस्थिति हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | हटाने के लिए निर्दिष्ट वस्तु। |

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
public final List<View> toList()
```


एक view संग्रह को [View](../../com.aspose.tasks/view) ऑब्जेक्ट्स की सूची में बदलता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - [View](../../com.aspose.tasks/view) वस्तुओं की सामान्य सूची।
