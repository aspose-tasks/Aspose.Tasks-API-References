---
title: "ResourceCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स का एक संग्रह दर्शाता है।"
type: docs
weight: 251
url: /hi/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

एक संग्रह को दर्शाता है जिसमें [Resource](../../com.aspose.tasks/resource) वस्तुएँ होती हैं।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add()](#add--) | परियोजना संसाधन संग्रह के अंतिम स्थान पर नया संसाधन जोड़ता है। |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | परियोजना संसाधन संग्रह के अंतिम स्थान पर नया संसाधन जोड़ता है। |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | परियोजना संसाधन संग्रह में निर्दिष्ट स्थिति पर नया संसाधन जोड़ता है। |
| [clear()](#clear--) | सीधे साफ़ करना समर्थित नहीं है, यह मेथड केवल UnsupportedOperationException फेंकता है। |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | निर्दिष्ट आईडी वाला संसाधन लौटाता है। |
| [getByUid(int uid)](#getByUid-int-) | निर्दिष्ट यूआईडी वाला संसाधन लौटाता है। |
| [getParentProject()](#getParentProject--) | ResourceCollection ऑब्जेक्ट का पैरेंट प्रोजेक्ट प्राप्त करता है। |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [remove(Object o)](#remove-java.lang.Object-) | यह Collection की remove मेथड का स्टब इम्प्लीमेंटेशन है, जो केवल UnsupportedOperationException फेंकता है। |
| [size()](#size--) | ResourceCollection में सम्मिलित तत्वों की संख्या प्राप्त करता है। |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | ResourceCollection ऑब्जेक्ट को [Resource](../../com.aspose.tasks/resource) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |
### add() {#add--}
```
public final Resource add()
```


परियोजना संसाधन संग्रह के अंतिम स्थान पर नया संसाधन जोड़ता है।

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


परियोजना संसाधन संग्रह के अंतिम स्थान पर नया संसाधन जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| resourceName | java.lang.String | संसाधन का नाम। |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


परियोजना संसाधन संग्रह में निर्दिष्ट स्थिति पर नया संसाधन जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| resourceName | java.lang.String | संसाधन का नाम। |
| beforeResourceId | int | परियोजना संसाधन संग्रह में पिछले संसाधन की स्थिति। |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


सीधे साफ़ करना समर्थित नहीं है, यह मेथड केवल UnsupportedOperationException फेंकता है।

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


निर्दिष्ट आईडी वाला संसाधन लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | id | int | निर्दिष्ट आईडी। |

--------------------

O(1) जटिलता। |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


निर्दिष्ट यूआईडी वाला संसाधन लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | uid | int | निर्दिष्ट uid। |

--------------------

O(1) जटिलता। |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceCollection ऑब्जेक्ट का पैरेंट प्रोजेक्ट प्राप्त करता है।

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```




**Returns:**
बूलियन - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - इस संग्रह के लिए एक इटरेटर।
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


यह Collection की remove मेथड का स्टब इम्प्लीमेंटेशन है, जो केवल UnsupportedOperationException फेंकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| o | java.lang.Object | हटाने के लिए आइटम। |

**Returns:**
boolean - यदि आइटम हटाया गया हो तो `true`; अन्यथा `false`।
### size() {#size--}
```
public final int size()
```


ResourceCollection में सम्मिलित तत्वों की संख्या प्राप्त करता है।

--------------------

केवल-पढ़ने योग्य `int`।

**Returns:**
int - ResourceCollection में सम्मिलित तत्वों की संख्या।
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


ResourceCollection ऑब्जेक्ट को [Resource](../../com.aspose.tasks/resource) ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - [Resource](../../com.aspose.tasks/resource) ऑब्जेक्ट्स की सूची।
