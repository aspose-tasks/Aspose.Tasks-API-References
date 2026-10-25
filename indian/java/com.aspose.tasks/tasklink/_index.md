---
title: "TaskLink"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक प्रीसेसर्स लिंक का प्रतिनिधित्व करता है।"
type: docs
weight: 295
url: /hi/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

एक प्रीसेसर्स लिंक का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [getCrossProjectName()](#getCrossProjectName--) | बाहरी पूर्वज प्रोजेक्ट प्राप्त करता है। |
| [getLagFormat()](#getLagFormat--) | लेग फ़ॉर्मेट को व्यक्त करने के लिए फ़ॉर्मेट प्राप्त करता है। |
| [getLinkLag()](#getLinkLag--) | एक मिनट के दसवें हिस्से या प्रतिशत में लेग प्राप्त करता है। |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | LagFormat के आधार पर लेग अवधि प्राप्त करता है। |
| [getLinkType()](#getLinkType--) | लिंक का प्रकार प्राप्त करता है। |
| [getPredTask()](#getPredTask--) | पूर्वज टास्क प्राप्त करता है। |
| [getSuccTask()](#getSuccTask--) | उत्तराधिकारी टास्क प्राप्त करता है। |
| [hashCode()](#hashCode--) | क्लास [TaskLink](../../com.aspose.tasks/tasklink) के इंस्टेंस के लिए हैश कोड मान लौटाता है। |
| [isCrossProject()](#isCrossProject--) | एक मान प्राप्त करता है जो दर्शाता है कि पूर्वज किसी अन्य प्रोजेक्ट का हिस्सा है या नहीं। |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | एक मान सेट करता है जो दर्शाता है कि पूर्वज किसी अन्य प्रोजेक्ट का हिस्सा है या नहीं। |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | बाहरी पूर्वज प्रोजेक्ट सेट करता है। |
| [setLagFormat(byte value)](#setLagFormat-byte-) | लेग फ़ॉर्मेट को व्यक्त करने के लिए फ़ॉर्मेट सेट करता है। |
| [setLinkLag(int value)](#setLinkLag-int-) | एक मिनट के दसवें हिस्से या प्रतिशत में लेग सेट करता है। |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | LagFormat के आधार पर लेग अवधि सेट करता है। |
| [setLinkType(int value)](#setLinkType-int-) | लिंक का प्रकार सेट करता है। |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | पूर्वज टास्क सेट करता है। |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | उत्तराधिकारी टास्क सेट करता है। |
| [toString()](#toString--) | TaskLink की स्ट्रिंग प्रतिनिधित्व लौटाता है। |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | इस इंस्टेंस की तुलना करने के लिए क्लास [TaskLink](../../com.aspose.tasks/tasklink) का निर्दिष्ट इंस्टेंस। |

**Returns:**
बूलियन - **True** यदि क्लास [TaskLink](../../com.aspose.tasks/tasklink) का निर्दिष्ट इंस्टेंस इस इंस्टेंस के समान पूर्वज और उत्तराधिकारी टास्क रखता है; अन्यथा, **false**।
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
बूलियन - **True** यदि निर्दिष्ट ऑब्जेक्ट एक TaskLink है जिसका पूर्वज और उत्तराधिकारी इस इंस्टेंस के समान है; अन्यथा, **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


बाहरी पूर्वज प्रोजेक्ट प्राप्त करता है।

**Returns:**
java.lang.String - बाहरी पूर्वज प्रोजेक्ट।
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


लेग फ़ॉर्मेट को व्यक्त करने के लिए फ़ॉर्मेट प्राप्त करता है।

**Returns:**
byte - विलंब स्वरूप को व्यक्त करने का प्रारूप।
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


एक मिनट के दसवें हिस्से या प्रतिशत में लेग प्राप्त करता है।

**Returns:**
int - मिनट के दशमलव हिस्से या प्रतिशत में विलंब।
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


LagFormat के आधार पर लेग अवधि प्राप्त करता है।

**Returns:**
double - विलंब अवधि, LagFormat पर निर्भर।
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


लिंक का प्रकार प्राप्त करता है।

**Returns:**
int - लिंक का प्रकार।
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


पूर्वज टास्क प्राप्त करता है।

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


उत्तराधिकारी टास्क प्राप्त करता है।

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


क्लास [TaskLink](../../com.aspose.tasks/tasklink) के इंस्टेंस के लिए हैश कोड मान लौटाता है।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


एक मान प्राप्त करता है जो दर्शाता है कि पूर्वज किसी अन्य प्रोजेक्ट का हिस्सा है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि क्या पूर्वज किसी अन्य प्रोजेक्ट का हिस्सा है।
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि पूर्वज किसी अन्य प्रोजेक्ट का हिस्सा है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि क्या पूर्वज किसी अन्य प्रोजेक्ट का हिस्सा है। |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


बाहरी पूर्वज प्रोजेक्ट सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | बाहरी पूर्वज प्रोजेक्ट। |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


लेग फ़ॉर्मेट को व्यक्त करने के लिए फ़ॉर्मेट सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | byte | विलंब स्वरूप को व्यक्त करने का प्रारूप। |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


एक मिनट के दसवें हिस्से या प्रतिशत में लेग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | मिनट के दशमलव हिस्से या प्रतिशत में विलंब। |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


LagFormat के आधार पर लेग अवधि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | विलंब अवधि, LagFormat पर निर्भर। |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


लिंक का प्रकार सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | लिंक का प्रकार। |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


पूर्वज टास्क सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | पूर्वज कार्य। |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


उत्तराधिकारी टास्क सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | उत्तराधिकारी कार्य। |

### toString() {#toString--}
```
public String toString()
```


TaskLink की स्ट्रिंग प्रतिनिधित्व लौटाता है। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और परिवर्तन के अधीन हो सकते हैं।

**Returns:**
java.lang.String - वह स्ट्रिंग जो TaskLink ऑब्जेक्ट का प्रतिनिधित्व करती है।
