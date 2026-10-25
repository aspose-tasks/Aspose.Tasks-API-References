---
title: "TaskBaseline"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "कार्य की बेसलाइन का प्रतिनिधित्व करता है।"
type: docs
weight: 291
url: /hi/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

कार्य की बेसलाइन का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | [TaskBaseline](../../com.aspose.tasks/taskbaseline) क्लास का नया उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | IComparable इंटरफ़ेस कार्यान्वयन। |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट TaskBaseline ऑब्जेक्ट के बराबर है या नहीं। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [getDuration()](#getDuration--) | जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित अवधि प्राप्त करता है। |
| [getEstimatedDuration()](#getEstimatedDuration--) | एक मान प्राप्त करता है जो दर्शाता है कि कार्य की बेसलाइन अवधि अनुमानित थी या नहीं। |
| [getFinish()](#getFinish--) | जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित समाप्ति तिथि प्राप्त करता है। |
| [getFixedCost()](#getFixedCost--) | जब बेसलाइन सहेजी गई थी, तब कार्य की स्थिर लागत प्राप्त करता है। |
| [getInterim()](#getInterim--) | एक मान प्राप्त करता है जो दर्शाता है कि यह एक अंतरिम बेसलाइन है या नहीं। |
| [getStart()](#getStart--) | जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित प्रारंभ तिथि प्राप्त करता है। |
| [getTimephasedData()](#getTimephasedData--) | इस ऑब्जेक्ट के लिए एक TimephasedDataCollection उदाहरण प्राप्त करता है। |
| [hashCode()](#hashCode--) | [TaskBaseline](../../com.aspose.tasks/taskbaseline) क्लास के उदाहरण के लिए एक हैश कोड मान लौटाता है। |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित अवधि सेट करता है। |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | एक मान सेट करता है जो दर्शाता है कि कार्य की बेसलाइन अवधि अनुमानित थी या नहीं। |
| [setFinish(Date value)](#setFinish-java.util.Date-) | जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित समाप्ति तिथि सेट करता है। |
| [setFixedCost(double value)](#setFixedCost-double-) | जब बेसलाइन सहेजी गई थी, तब कार्य की निश्चित लागत सेट करता है। |
| [setInterim(boolean value)](#setInterim-boolean-) | यह एक अंतरिम बेसलाइन है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setStart(Date value)](#setStart-java.util.Date-) | जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित प्रारंभ तिथि सेट करता है। |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | इस ऑब्जेक्ट के लिए एक TimephasedDataCollection इंस्टेंस सेट करता है। |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


[TaskBaseline](../../com.aspose.tasks/taskbaseline) क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | बेसलाइन का मूल कार्य। |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


IComparable इंटरफ़ेस कार्यान्वयन। इस इंस्टेंस की निर्दिष्ट Baseline ऑब्जेक्ट से तुलना करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | इस इंस्टेंस की तुलना करने के लिए निर्दिष्ट Baseline ऑब्जेक्ट। |

**Returns:**
int - यदि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से कम है तो -1 लौटाता है, यदि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है तो 1; अन्यथा 0 लौटाता है।
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट TaskBaseline ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | इस इंस्टेंस से तुलना करने के लिए निर्दिष्ट AssignmentBaseline ऑब्जेक्ट। |

**Returns:**
बूलियन - यदि यह इंस्टेंस निर्दिष्ट TaskBaseline ऑब्जेक्ट के बराबर है तो true लौटाता है; अन्यथा false।
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | इस इंस्टेंस की तुलना करने के लिए ऑब्जेक्ट। |

**Returns:**
बूलियन - यदि निर्दिष्ट ऑब्जेक्ट एक TaskBaseline है जिसका UID मान इस इंस्टेंस के समान है तो **True**; अन्यथा **false**।
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित अवधि प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


एक मान प्राप्त करता है जो दर्शाता है कि कार्य की बेसलाइन अवधि अनुमानित थी या नहीं।

**Returns:**
बूलियन - यह दर्शाने वाला मान कि कार्य की बेसलाइन अवधि अनुमानित थी या नहीं।
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित समाप्ति तिथि प्राप्त करता है।

**Returns:**
java.util.Date - जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित समाप्ति तिथि।
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


जब बेसलाइन सहेजी गई थी, तब कार्य की स्थिर लागत प्राप्त करता है।

**Returns:**
double - जब बेसलाइन सहेजी गई थी, तब कार्य की निश्चित लागत।
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


एक मान प्राप्त करता है जो दर्शाता है कि यह एक अंतरिम बेसलाइन है या नहीं।

**Returns:**
बूलियन - यह दर्शाने वाला मान कि यह एक अंतरिम बेसलाइन है या नहीं।
### getStart() {#getStart--}
```
public final Date getStart()
```


जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित प्रारंभ तिथि प्राप्त करता है।

**Returns:**
java.util.Date - जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित प्रारंभ तिथि।
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


इस ऑब्जेक्ट के लिए एक TimephasedDataCollection इंस्टेंस प्राप्त करता है। कार्य बेसलाइन से जुड़ा समय-फ़ेज़्ड डेटा।

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[TaskBaseline](../../com.aspose.tasks/taskbaseline) क्लास के उदाहरण के लिए एक हैश कोड मान लौटाता है।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित अवधि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित अवधि। |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि कार्य की बेसलाइन अवधि अनुमानित थी या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | यह दर्शाने वाला मान कि कार्य की बेसलाइन अवधि अनुमानित थी या नहीं। |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित समाप्ति तिथि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित समाप्ति तिथि। |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


जब बेसलाइन सहेजी गई थी, तब कार्य की निश्चित लागत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | जब बेसलाइन सहेजी गई थी, तब कार्य की निश्चित लागत। |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


यह एक अंतरिम बेसलाइन है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | यह दर्शाने वाला मान कि यह एक अंतरिम बेसलाइन है या नहीं। |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित प्रारंभ तिथि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | जब बेसलाइन सहेजी गई थी, तब कार्य की नियोजित प्रारंभ तिथि। |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


इस ऑब्जेक्ट के लिए एक TimephasedDataCollection इंस्टेंस सेट करता है। कार्य बेसलाइन से जुड़ा समय-फ़ेज़्ड डेटा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | इस ऑब्जेक्ट के लिए एक TimephasedDataCollection इंस्टेंस। |

