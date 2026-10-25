---
title: "WorkingTime"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "कार्यदिवस के दौरान कार्य समय का प्रतिनिधित्व करता है।"
type: docs
weight: 365
url: /hi/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

कार्यदिवस के दौरान कार्य समय का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | नए उदाहरण को [WorkingTime](../../com.aspose.tasks/workingtime) क्लास का एक अंतराल के साथ प्रारंभ करता है, जिसमें निर्दिष्ट प्रारंभ और समाप्ति समय होते हैं। |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | नए उदाहरण को [WorkingTime](../../com.aspose.tasks/workingtime) क्लास का एक अंतराल आइटम के साथ प्रारंभ करता है, जिसमें निर्दिष्ट प्रारंभ और समाप्ति समय होते हैं। |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | नए उदाहरण को [WorkingTime](../../com.aspose.tasks/workingtime) क्लास का एक अंतराल आइटम के साथ प्रारंभ करता है, जिसमें निर्दिष्ट प्रारंभ और समाप्ति समय होते हैं। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | जाँचता है कि वस्तुएँ समान हैं। |
| [getFrom()](#getFrom--) | कार्य समय की शुरुआत प्राप्त करता है। |
| [getTo()](#getTo--) | कार्य समय का अंत प्राप्त करता है। |
| [hashCode()](#hashCode--) | वापस करता है [WorkingTime](../../com.aspose.tasks/workingtime) क्लास के उदाहरण के लिए हैश कोड मान। |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


नए उदाहरण को [WorkingTime](../../com.aspose.tasks/workingtime) क्लास का एक अंतराल के साथ प्रारंभ करता है, जिसमें निर्दिष्ट प्रारंभ और समाप्ति समय होते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fromTime | java.util.Date | अंतराल प्रारंभ समय |
| toTime | java.util.Date | अंतराल समाप्ति समय |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


नए उदाहरण को [WorkingTime](../../com.aspose.tasks/workingtime) क्लास का एक अंतराल आइटम के साथ प्रारंभ करता है, जिसमें निर्दिष्ट प्रारंभ और समाप्ति समय होते हैं।

--------------------

&gt; ```
&gt; WorkingTime ctor का ओवरलोड अंतराल की शुरुआत और अंत को TimeSpans का उपयोग करके प्रारंभ करने के लिए उपयोग किया जा सकता है:
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fromHours | int | अंतराल की शुरुआत का समय पूरे घंटे (0-24) में दर्शाया गया है। |
| toHours | int | अंतराल के अंत का समय पूरे घंटे (0-24) में दर्शाया गया है। |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


जाँचता है कि वस्तुएँ समान हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | तुलना करने के लिए दूसरी वस्तु। |

**Returns:**
boolean - यदि वस्तुएँ समान हैं तो True, अन्यथा false।
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


कार्य समय की शुरुआत प्राप्त करता है।

**Returns:**
java.util.Date - कार्य समय की शुरुआत।
### getTo() {#getTo--}
```
public final Date getTo()
```


कार्य समय का अंत प्राप्त करता है।

**Returns:**
java.util.Date - कार्य समय का अंत।
### hashCode() {#hashCode--}
```
public int hashCode()
```


वापस करता है [WorkingTime](../../com.aspose.tasks/workingtime) क्लास के उदाहरण के लिए हैश कोड मान।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
