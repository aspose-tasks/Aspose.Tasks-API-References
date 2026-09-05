---
title: "SimpleSaveOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "यह एक अमूर्त बेस क्लास है जो उपयोगकर्ता को किसी विशिष्ट फ़ॉर्मेट में परियोजना सहेजते समय बुनियादी विकल्प निर्दिष्ट करने की अनुमति देती है।"
type: docs
weight: 277
url: /hi/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

यह एक अमूर्त बेस क्लास है जो उपयोगकर्ता को किसी विशिष्ट फ़ॉर्मेट में परियोजना सहेजते समय बुनियादी विकल्प निर्दिष्ट करने की अनुमति देती है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | यदि इस सहेजने विकल्प ऑब्जेक्ट का उपयोग किया जाता है तो दस्तावेज़ किस फ़ॉर्मेट में सहेजा जाएगा, यह प्राप्त करता है। |
| [getTasksComparer()](#getTasksComparer--) | Gantt चार्ट और Task Sheet चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को प्राप्त करता है। |
| [getTasksFilter()](#getTasksFilter--) | Gantt, Task Sheet और Task Usage चार्ट पर प्रदर्शित कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त प्राप्त करता है। |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Gantt चार्ट और Task Sheet चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को सेट करता है। |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Gantt, Task Sheet और Task Usage चार्ट पर प्रदर्शित कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त सेट करता है। |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


यदि इस सहेजने विकल्प ऑब्जेक्ट का उपयोग किया जाता है तो दस्तावेज़ किस फ़ॉर्मेट में सहेजा जाएगा, यह प्राप्त करता है।

**Returns:**
int - वह [SaveFileFormat](../../com.aspose.tasks/savefileformat) जिसमें दस्तावेज़ सहेजा जाएगा।
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Gantt चार्ट और Task Sheet चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को प्राप्त करता है।

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - Gantt चार्ट और Task Sheet चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाला।
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Gantt, Task Sheet और Task Usage चार्ट पर प्रदर्शित कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त प्राप्त करता है।

--------------------

यदि मान निर्दिष्ट नहीं किया गया है तो डिफ़ॉल्ट फ़िल्टर उपयोग किया जाता है जो अदृश्य कार्यों को हटाता है — अर्थात् संकुचित कार्यों की संतति कार्य।

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Gantt चार्ट और Task Sheet चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाले को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | Gantt चार्ट और Task Sheet चार्ट पर कार्यों को क्रमबद्ध करने के लिए तुलना करने वाला। |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Gantt, Task Sheet और Task Usage चार्ट पर प्रदर्शित कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त सेट करता है।

--------------------

यदि मान निर्दिष्ट नहीं किया गया है तो डिफ़ॉल्ट फ़िल्टर उपयोग किया जाता है जो अदृश्य कार्यों को हटाता है — अर्थात् संकुचित कार्यों की संतति कार्य।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Gantt, Task Sheet और Task Usage चार्ट पर रेंडर किए गए कार्यों को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त। |

