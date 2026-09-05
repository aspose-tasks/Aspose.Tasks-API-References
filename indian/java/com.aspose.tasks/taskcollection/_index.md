---
title: "TaskCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स का एक संग्रह दर्शाता है।"
type: docs
weight: 293
url: /hi/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

एक संग्रह का प्रतिनिधित्व करता है जिसमें [Task](../../com.aspose.tasks/task) वस्तुएँ होती हैं।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add()](#add--) | पिछले कार्य के समान रूपरेखा स्तर पर प्रोजेक्ट कार्य संग्रह में नया कार्य जोड़ता है। |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | निर्दिष्ट आईडी वाले कार्य से पहले और समान रूपरेखा स्तर पर नया कार्य सम्मिलित करता है। |
| [add(Task item)](#add-com.aspose.tasks.Task-) | निर्दिष्ट कार्य को [TaskCollection](../../com.aspose.tasks/taskcollection) क्लास के उदाहरण में जोड़ें। |
| [add(String taskName)](#add-java.lang.String-) | चाइल्ड कार्य संग्रह में नया कार्य जोड़ता है। |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | चाइल्ड कार्य संग्रह में नया आवर्ती कार्य जोड़ता है। |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | जाँचता है कि संग्रह में निर्दिष्ट आइटम मौजूद है या नहीं। |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | एक कार्य लौटाता है जिसका निर्दिष्ट Id है और जिसका पूर्वज इस संग्रह का पैरेंट कार्य है। |
| [getByUid(int uid)](#getByUid-int-) | एक कार्य लौटाता है जिसका निर्दिष्ट Uid है और जिसका पूर्वज इस संग्रह का पैरेंट कार्य है। |
| [getParentProject()](#getParentProject--) | TaskCollection वस्तु का पैरेंट प्रोजेक्ट प्राप्त करता है। |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं। |
| [iterator()](#iterator--) | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [remove(Object item)](#remove-java.lang.Object-) | यह ICollection के Remove मेथड की स्टब कार्यान्वयन है, जो केवल UnsupportedOperationException फेंकता है। |
| [size()](#size--) | TaskCollection में सम्मिलित वस्तुओं की संख्या प्राप्त करता है। |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | TaskCollection वस्तु को [Task](../../com.aspose.tasks/task) वस्तुओं की सूची में परिवर्तित करता है। |
### add() {#add--}
```
public final Task add()
```


पिछले कार्य के समान रूपरेखा स्तर पर प्रोजेक्ट कार्य संग्रह में नया कार्य जोड़ता है।

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


निर्दिष्ट आईडी वाले कार्य से पहले और समान रूपरेखा स्तर पर नया कार्य सम्मिलित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | आवर्ती कार्य बनाने के लिए निर्दिष्ट पैरामीटर। |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


निर्दिष्ट कार्य को [TaskCollection](../../com.aspose.tasks/taskcollection) क्लास की इंस्टेंस में जोड़ें। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस मेथड का उपयोग करने के बाद Project.Recalculate() को कॉल करना चाहिए (यह सभी प्रोजेक्ट कार्यों (शुरू/समाप्ति तिथियों, प्रारंभिक/अंतिम तिथियों को सेट करता है) को पुनः शेड्यूल करेगा और स्लैक, कार्य और लागत फ़ील्ड, आईडी और रूपरेखा स्तर जैसे निर्भर फ़ील्ड की गणना करेगा)। यदि ParentProject.CalculationMode Manual है तो मेथड केवल कार्य आईडी, रूपरेखा स्तर और रूपरेखा संख्याओं की स्वचालित रूप से गणना करेगा। यदि ParentProject.CalculationMode Automatic है तो मेथड सभी प्रोजेक्ट कार्यों को स्वचालित रूप से पुनः शेड्यूल करेगा (शुरू/समाप्ति तिथियों, प्रारंभिक/अंतिम तिथियों को सेट करता है, स्लैक, कार्य और लागत फ़ील्ड की गणना करता है, आईडी और रूपरेखा स्तर को पुनः गणना करता है)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | निर्दिष्ट कार्य जिसे इस कार्य संग्रह में जोड़ा जाना चाहिए। |

**Returns:**
boolean - यदि ऑपरेशन सफल रहा तो true।
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


चाइल्ड कार्य संग्रह में नया कार्य जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| taskName | java.lang.String | निर्दिष्ट कार्य नाम। |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


चाइल्ड कार्य संग्रह में नया आवर्ती कार्य जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| taskName | java.lang.String | निर्दिष्ट कार्य नाम। |
| beforeTaskId | int | निर्दिष्ट आईडी वह है जिसके पहले एक नया कार्य सम्मिलित किया जाएगा। |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns a task which was inserted before a task with the specified id.
### clear() {#clear--}
```
public final void clear()
```




### contains(Task item) {#contains-com.aspose.tasks.Task-}
```
public final boolean contains(Task item)
```


जाँचता है कि संग्रह में निर्दिष्ट आइटम मौजूद है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | जाँचने के लिए आइटम। |

**Returns:**
boolean - true, यदि संग्रह में कोई आइटम हो, अन्यथा false।
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


एक कार्य लौटाता है जिसका निर्दिष्ट Id है और जिसका पूर्वज इस संग्रह का पैरेंट कार्य है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


एक कार्य लौटाता है जिसका निर्दिष्ट Uid है और जिसका पूर्वज इस संग्रह का पैरेंट कार्य है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


TaskCollection वस्तु का पैरेंट प्रोजेक्ट प्राप्त करता है।

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
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
public final Iterator<Task> iterator()
```


इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - इस संग्रह के लिए एक इटरेटर।
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


यह ICollection के Remove मेथड की स्टब कार्यान्वयन है, जो केवल UnsupportedOperationException फेंकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | java.lang.Object | हटाने के लिए आइटम। |

**Returns:**
boolean - यदि आइटम हटाया गया हो तो `true`; अन्यथा `false`।
### size() {#size--}
```
public final int size()
```


TaskCollection में सम्मिलित वस्तुओं की संख्या प्राप्त करता है।

**Returns:**
int - TaskCollection में सम्मिलित वस्तुओं की संख्या।
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


TaskCollection वस्तु को [Task](../../com.aspose.tasks/task) वस्तुओं की सूची में परिवर्तित करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - एक सूची लौटाता है जिसमें इस संग्रह की [Task](../../com.aspose.tasks/task) क्लास की इंस्टेंसेज़ शामिल हैं।
