---
title: "CalendarCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स का एक संग्रह दर्शाता है।"
type: docs
weight: 42
url: /hi/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

एक संग्रह का प्रतिनिधित्व करता है जिसमें [Calendar](../../com.aspose.tasks/calendar) वस्तुएँ होती हैं।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | इस CalendarCollection ऑब्जेक्ट में एक नया बेस कैलेंडर जोड़ता है और जोड़ा गया कैलेंडर लौटाता है। |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | निर्दिष्ट बेस कैलेंडर के साथ एक नया कैलेंडर इस CalendarCollection ऑब्जेक्ट में जोड़ता है और जोड़ा गया कैलेंडर लौटाता है। |
| [clear()](#clear--) | इस संग्रह से सभी तत्वों को हटा देता है। |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | निर्दिष्ट नाम वाले कैलेंडर को लौटाता है। |
| [getByUid(int uid)](#getByUid-int-) | निर्दिष्ट UID वाले कैलेंडर को लौटाता है। |
| [iterator()](#iterator--) | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [remove(int index)](#remove-int-) | इस सूची में निर्दिष्ट स्थिति पर तत्व को हटाता है। |
| [remove(Object item)](#remove-java.lang.Object-) | प्रोजेक्ट CalendarCollection से कैलेंडर को हटाता है। |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | इस सूची में निर्दिष्ट स्थिति पर तत्व को निर्दिष्ट तत्व से बदलता है। |
| [size()](#size--) | इस [CalendarCollection](../../com.aspose.tasks/calendarcollection) ऑब्जेक्ट में मौजूद वस्तुओं की संख्या प्राप्त करता है। |
| [toList()](#toList--) | CalendarCollection ऑब्जेक्ट को [Calendar](../../com.aspose.tasks/calendar) वस्तुओं की सूची में परिवर्तित करता है। |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


इस CalendarCollection ऑब्जेक्ट में एक नया बेस कैलेंडर जोड़ता है और जोड़ा गया कैलेंडर लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | कैलेंडर का नाम। |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


निर्दिष्ट बेस कैलेंडर के साथ एक नया कैलेंडर इस CalendarCollection ऑब्जेक्ट में जोड़ता है और जोड़ा गया कैलेंडर लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | निर्दिष्ट नाम। |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | निर्दिष्ट बेस कैलेंडर। |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


इस संग्रह से सभी तत्वों को हटा देता है।

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


निर्दिष्ट नाम वाले कैलेंडर को लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | कैलेंडर का नाम। |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


निर्दिष्ट UID वाले कैलेंडर को लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uid | int | कैलेंडर का UID। |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - इस संग्रह के लिए एक इटेरेटर।
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


इस सूची में निर्दिष्ट स्थिति पर तत्व को हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


प्रोजेक्ट CalendarCollection से कैलेंडर को हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | java.lang.Object | हटाने के लिए कैलेंडर। |

**Returns:**
boolean - यदि हटाया गया तो true लौटाता है, अन्यथा false।
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


इस सूची में निर्दिष्ट स्थिति पर तत्व को निर्दिष्ट तत्व से बदलता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


इस [CalendarCollection](../../com.aspose.tasks/calendarcollection) ऑब्जेक्ट में मौजूद वस्तुओं की संख्या प्राप्त करता है।

**Returns:**
int - इस [CalendarCollection](../../com.aspose.tasks/calendarcollection) ऑब्जेक्ट में मौजूद वस्तुओं की संख्या।
### toList() {#toList--}
```
public final List<Calendar> toList()
```


CalendarCollection ऑब्जेक्ट को [Calendar](../../com.aspose.tasks/calendar) वस्तुओं की सूची में परिवर्तित करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - [Calendar](../../com.aspose.tasks/calendar) वस्तुओं की सूची।
