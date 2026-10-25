---
title: "TaskLinkCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स का एक संग्रह दर्शाता है।"
type: docs
weight: 296
url: /hi/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

एक संग्रह का प्रतिनिधित्व करता है जिसमें [Task](../../com.aspose.tasks/task) वस्तुएँ होती हैं।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | एक Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) का उदाहरण लौटाता है जो TaskLinkCollection वस्तु में जोड़ा गया है। |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | एक [TaskLink](../../com.aspose.tasks/tasklink) का उदाहरण लौटाता है जो TaskLinkCollection वस्तु में जोड़ा गया है। |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | एक [TaskLink](../../com.aspose.tasks/tasklink) का उदाहरण लौटाता है जो TaskLinkCollection वस्तु में जोड़ा गया है। |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | यह ICollection के Add मेथड की स्टब कार्यान्वयन है, जो केवल UnsupportedOperationException फेंकता है। |
| [clear()](#clear--) | आंतरिक उपयोग के लिए आरक्षित। |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | ResourceAssignmentCollection वस्तु का पैरेंट प्रोजेक्ट प्राप्त करता है। |
| [remove(int index)](#remove-int-) | इस संग्रह में निर्दिष्ट स्थिति पर तत्व को हटाता है और हटाए गए तत्व को लौटाता है। |
| [remove(Object item)](#remove-java.lang.Object-) | एक प्रोजेक्ट से टास्क लिंक हटाता है। |
| [size()](#size--) | इस `TaskLinkCollection` वस्तु में मौजूद वस्तुओं की संख्या लौटाता है। |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | TaskLinkCollection वस्तु को [TaskLink](../../com.aspose.tasks/tasklink) वस्तुओं की सूची में परिवर्तित करता है। |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


एक Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) का उदाहरण लौटाता है जो TaskLinkCollection वस्तु में जोड़ा गया है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | पूर्ववर्ती कार्य। |
| succ | [Task](../../com.aspose.tasks/task) | उत्तराधिकारी कार्य। |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


एक [TaskLink](../../com.aspose.tasks/tasklink) का उदाहरण लौटाता है जो TaskLinkCollection वस्तु में जोड़ा गया है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | पूर्ववर्ती कार्य। |
| succ | [Task](../../com.aspose.tasks/task) | उत्तराधिकारी कार्य। |
| linkType | int | लिंक प्रकार [TaskLinkType](../../com.aspose.tasks/tasklinktype)। |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


एक [TaskLink](../../com.aspose.tasks/tasklink) का उदाहरण लौटाता है जो TaskLinkCollection वस्तु में जोड़ा गया है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | पूर्ववर्ती कार्य। |
| succ | [Task](../../com.aspose.tasks/task) | उत्तराधिकारी कार्य। |
| linkType | int | लिंक प्रकार [TaskLinkType](../../com.aspose.tasks/tasklinktype)। |
| lag | [Duration](../../com.aspose.tasks/duration) | लिंक लैग [Duration](../../com.aspose.tasks/duration)। |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


यह ICollection के Add मेथड की स्टब कार्यान्वयन है, जो केवल UnsupportedOperationException फेंकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | जोड़ने के लिए आइटम। |

**Returns:**
बूलियन - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


आंतरिक उपयोग के लिए आरक्षित।

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceAssignmentCollection वस्तु का पैरेंट प्रोजेक्ट प्राप्त करता है।

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


इस संग्रह में निर्दिष्ट स्थिति पर तत्व को हटाता है और हटाए गए तत्व को लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | तत्व को हटाने के लिए निर्दिष्ट स्थिति। |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


एक प्रोजेक्ट से टास्क लिंक हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | java.lang.Object | हटाने के लिए `TaskLink` क्लास का निर्दिष्ट उदाहरण। |

**Returns:**
boolean - इस संग्रह से हटाए गए `TaskLink` क्लास के उदाहरण को लौटाता है।
### size() {#size--}
```
public final int size()
```


इस `TaskLinkCollection` वस्तु में मौजूद वस्तुओं की संख्या लौटाता है। केवल-पढ़ने योग्य `int`।

**Returns:**
int - इस संग्रह में मौजूद वस्तुओं की संख्या लौटाता है।
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


TaskLinkCollection वस्तु को [TaskLink](../../com.aspose.tasks/tasklink) वस्तुओं की सूची में परिवर्तित करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - [TaskLink](../../com.aspose.tasks/tasklink) वस्तुओं की सूची।
