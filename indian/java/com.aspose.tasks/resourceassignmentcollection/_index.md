---
title: "ResourceAssignmentCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स का एक संग्रह दर्शाता है।"
type: docs
weight: 250
url: /hi/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

[ResourceAssignment](../../com.aspose.tasks/resourceassignment) ऑब्जेक्ट्स का संग्रह दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | यह ICollection के Add मेथड की स्टब कार्यान्वयन है, जो केवल UnsupportedOperationException फेंकता है। |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है। |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है। |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है। |
| [clear()](#clear--) | संग्रह से सभी आइटम हटाता है। |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | निर्दिष्ट uid वाला असाइनमेंट लौटाता है। |
| [getParentProject()](#getParentProject--) | ResourceAssignmentCollection वस्तु का पैरेंट प्रोजेक्ट प्राप्त करता है। |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं। |
| [iterator()](#iterator--) | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | यदि संग्रह केवल-पढ़ने योग्य नहीं है तो निर्दिष्ट असाइनमेंट को हटाता है, अन्यथा UnsupportedOperationException फेंकता है। |
| [size()](#size--) | ResourceAssignmentCollection में शामिल ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [toList()](#toList--) | ResourceAssignmentCollection ऑब्जेक्ट को [ResourceAssignment](../../com.aspose.tasks/resourceassignment) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


यह ICollection के Add मेथड की स्टब कार्यान्वयन है, जो केवल UnsupportedOperationException फेंकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | हटाने के लिए आइटम। |

**Returns:**
बूलियन - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | एक कार्य जिसे असाइन किया जाना है। |
| resource | [Resource](../../com.aspose.tasks/resource) | एक संसाधन जिसे असाइन किया जाना है। |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | एक कार्य जिसे असाइन किया जाना है। |
| resource | [Resource](../../com.aspose.tasks/resource) | एक संसाधन जिसे असाइन किया जाना है। |
| इकाइयाँ | double | नए असाइनमेंट के लिए इकाइयों की संख्या। |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | एक कार्य जिसे असाइन किया जाना है। |
| resource | [Resource](../../com.aspose.tasks/resource) | एक लागत संसाधन जिसे असाइन किया जाना है। |
| लागत | java.math.BigDecimal | नए असाइनमेंट की लागत। |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


संग्रह से सभी आइटम हटाता है।

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
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


निर्दिष्ट uid वाला असाइनमेंट लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | uid | int | निर्दिष्ट uid। |

--------------------

O(1) जटिलता। |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceAssignmentCollection वस्तु का पैरेंट प्रोजेक्ट प्राप्त करता है।

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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


एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं।
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - इस संग्रह के लिए एक एन्यूमरेटर।
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


यदि संग्रह केवल-पढ़ने योग्य नहीं है तो निर्दिष्ट असाइनमेंट को हटाता है, अन्यथा UnsupportedOperationException फेंकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| o | java.lang.Object | हटाने के लिए असाइनमेंट। |

**Returns:**
boolean - true, यदि निर्दिष्ट आइटम हटाया गया हो, अन्यथा false।
### size() {#size--}
```
public final int size()
```


ResourceAssignmentCollection में शामिल ऑब्जेक्ट्स की संख्या प्राप्त करता है।

**Returns:**
int - ResourceAssignmentCollection में मौजूद ऑब्जेक्ट्स की संख्या।
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


ResourceAssignmentCollection ऑब्जेक्ट को [ResourceAssignment](../../com.aspose.tasks/resourceassignment) ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - [ResourceAssignment](../../com.aspose.tasks/resourceassignment) ऑब्जेक्ट्स की सूची।
