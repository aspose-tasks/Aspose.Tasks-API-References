---
title: "Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट पृष्ठों को Spreadsheet2003 में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 280
url: /hi/java/com.aspose.tasks/spreadsheet2003saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class Spreadsheet2003SaveOptions extends SimpleSaveOptions
```

प्रोजेक्ट पृष्ठों को Spreadsheet2003 में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Spreadsheet2003SaveOptions()](#Spreadsheet2003SaveOptions--) | एक नया उदाहरण प्रारंभ करता है [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची प्राप्त करता है ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getResourceView()](#getResourceView--) | रेंडर करने के लिए संसाधन दृश्य कॉलम की सूची प्राप्त करता है ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | सहेजने के लिए दृश्य कॉलम की सूची प्राप्त करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची सेट करता है ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | रेंडर करने के लिए संसाधन दृश्य कॉलम की सूची सेट करता है ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | सहेजने के लिए दृश्य कॉलम की सूची सेट करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
### Spreadsheet2003SaveOptions() {#Spreadsheet2003SaveOptions--}
```
public Spreadsheet2003SaveOptions()
```


एक नया उदाहरण प्रारंभ करता है [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) क्लास का।

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची प्राप्त करता है ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
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


सहेजने के लिए दृश्य कॉलम की सूची प्राप्त करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं।

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची सेट करता है ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | रेंडर करने के लिए असाइनमेंट्स दृश्य कॉलम की सूची ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

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


सहेजने के लिए दृश्य कॉलम की सूची सेट करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | सहेजने के लिए दृश्य कॉलम की सूची ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

