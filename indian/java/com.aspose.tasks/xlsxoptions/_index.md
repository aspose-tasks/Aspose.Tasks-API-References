---
title: "XlsxOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट पेजों को XLSX में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 368
url: /hi/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

प्रोजेक्ट पेजों को XLSX में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | नया उदाहरण प्रारंभ करता है [XlsxOptions](../../com.aspose/tasks/xlsxoptions) क्लास का, जिसका उपयोग प्रोजेक्ट को XLSX फ़ॉर्मेट में सहेजने के लिए किया जा सकता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची प्राप्त करता है ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | परिणामी XLSX फ़ाइल की एन्कोडिंग प्राप्त करता है। |
| [getResourceView()](#getResourceView--) | रेंडर करने के लिए संसाधन दृश्य कॉलम की सूची प्राप्त करता है ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची प्राप्त करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))। |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची सेट करता है ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | परिणामी XLSX फ़ाइल की एन्कोडिंग सेट करता है। |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | रेंडर करने के लिए संसाधन दृश्य कॉलम की सूची सेट करता है ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची सेट करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))। |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


नया उदाहरण प्रारंभ करता है [XlsxOptions](../../com.aspose/tasks/xlsxoptions) क्लास का, जिसका उपयोग प्रोजेक्ट को XLSX फ़ॉर्मेट में सहेजने के लिए किया जा सकता है।

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची प्राप्त करता है ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


परिणामी XLSX फ़ाइल की एन्कोडिंग प्राप्त करता है। डिफ़ॉल्ट मान है java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset - परिणामी XLSX फ़ाइल की एन्कोडिंग।
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


रेंडर करने के लिए संसाधन दृश्य कॉलम की सूची प्राप्त करता है ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची प्राप्त करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))। यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं।

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची सेट करता है ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


परिणामी XLSX फ़ाइल की एन्कोडिंग सेट करता है। डिफ़ॉल्ट मान है java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.nio.charset.Charset | परिणामी XLSX फ़ाइल की एन्कोडिंग। |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


रेंडर करने के लिए संसाधन दृश्य कॉलम की सूची सेट करता है ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | रेंडर करने के लिए संसाधन दृश्य कॉलम की सूची ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची सेट करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))। यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची। ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) |

