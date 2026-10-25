---
title: "GanttChartColumn"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Projects व्यू क्लास"
type: docs
weight: 111
url: /hi/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

प्रोजेक्ट का दृश्य वर्ग
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | वर्तमान टास्क को कॉलम टेक्स्ट में बदलता है। |
| [getField()](#getField--) | कॉलम फ़ील्ड लौटाता है। |
| [setField(int value)](#setField-int-) | कॉलम फ़ील्ड सेट करता है। |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | कॉलम का नाम। |
| width | int | पिक्सेल में कॉलम की चौड़ाई। |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | टास्क डेटा को कॉलम टेक्स्ट में परिवर्तित करने वाला कन्वर्टर। |
| फ़ील्ड | int | कॉलम फ़ील्ड। |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | कॉलम का नाम। |
| width | int | पिक्सेल में कॉलम की चौड़ाई। |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | टास्क डेटा को कॉलम टेक्स्ट में परिवर्तित करने वाला कन्वर्टर। |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| width | int | पिक्सेल में कॉलम की चौड़ाई। |
| फ़ील्ड | int | कॉलम फ़ील्ड। |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


GanttChartColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | कॉलम का नाम। |
| width | int | पिक्सेल में कॉलम की चौड़ाई। |
| फ़ील्ड | int | कॉलम फ़ील्ड। |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


वर्तमान टास्क को कॉलम टेक्स्ट में बदलता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | वर्तमान टास्क। |

**Returns:**
java.lang.String - कॉलम टेक्स्ट।
### getField() {#getField--}
```
public int getField()
```


कॉलम फ़ील्ड लौटाता है। `Field`.

**Returns:**
int - कॉलम फ़ील्ड मान।
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


कॉलम फ़ील्ड सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | कॉलम फ़ील्ड मान। |

