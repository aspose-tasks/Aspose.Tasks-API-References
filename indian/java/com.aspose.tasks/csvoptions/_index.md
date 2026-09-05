---
title: "CsvOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट को CSV में सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 56
url: /hi/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

प्रोजेक्ट को CSV में सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | एक नया उदाहरण प्रारंभ करता है [CsvOptions](../../com.aspose/tasks/csvoptions) क्लास का, जिसका उपयोग प्रोजेक्ट को CSV फ़ॉर्मेट में सहेजने के लिए किया जा सकता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | सहेजे जाने वाले डेटा श्रेणी को प्राप्त करता है। |
| [getEncoding()](#getEncoding--) | CSV को सहेजने के लिए उपयोग की जाने वाली एन्कोडिंग प्राप्त करता है। |
| [getIncludeHeaders()](#getIncludeHeaders--) | हेडर शामिल करने हैं या नहीं, यह दर्शाने वाला मान प्राप्त करता है (डिफ़ॉल्ट मान TRUE है)। |
| [getTextDelimiter()](#getTextDelimiter--) | टेक्स्ट डिलिमिटर प्राप्त करता है। |
| [getView()](#getView--) | XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची प्राप्त करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))। |
| [setDataCategory(int value)](#setDataCategory-int-) | सहेजे जाने वाले डेटा श्रेणी को सेट करता है। |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | CSV को सहेजने के लिए एन्कोडिंग सेट करता है। |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | हेडर शामिल करने हैं या नहीं, यह दर्शाने वाला मान सेट करता है (डिफ़ॉल्ट मान TRUE है)। |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | टेक्स्ट डिलिमिटर सेट करता है। |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची सेट करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))। |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


एक नया उदाहरण प्रारंभ करता है [CsvOptions](../../com.aspose/tasks/csvoptions) क्लास का, जिसका उपयोग प्रोजेक्ट को CSV फ़ॉर्मेट में सहेजने के लिए किया जा सकता है।

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


सहेजे जाने वाले डेटा श्रेणी को प्राप्त करता है।

**Returns:**
int - सहेजे जाने वाला डेटा श्रेणी।
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


CSV को सहेजने के लिए उपयोग की जाने वाली एन्कोडिंग प्राप्त करता है।

**Returns:**
java.nio.charset.Charset - CSV को सहेजने के लिए एन्कोडिंग।
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


हेडर शामिल करने हैं या नहीं, यह दर्शाने वाला मान प्राप्त करता है (डिफ़ॉल्ट मान TRUE है)।

**Returns:**
boolean - हेडर शामिल करने हैं या नहीं, यह दर्शाने वाला मान (डिफ़ॉल्ट मान TRUE है)।
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


टेक्स्ट डिलिमिटर प्राप्त करता है।

**Returns:**
int - टेक्स्ट डिलिमिटर।
### getView() {#getView--}
```
public final ProjectView getView()
```


XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची प्राप्त करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))। यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं।

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


सहेजे जाने वाले डेटा श्रेणी को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | सहेजे जाने वाला डेटा श्रेणी। |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


CSV को सहेजने के लिए एन्कोडिंग सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.nio.charset.Charset | CSV को सहेजने के लिए एन्कोडिंग। |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


हेडर शामिल करने हैं या नहीं, यह दर्शाने वाला मान सेट करता है (डिफ़ॉल्ट मान TRUE है)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | हेडर शामिल करने हैं या नहीं, यह दर्शाने वाला मान (डिफ़ॉल्ट मान TRUE है)। |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


टेक्स्ट डिलिमिटर सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | टेक्स्ट डिलिमिटर। |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची सेट करता है ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))। यदि सेट नहीं किया गया तो डिफ़ॉल्ट कॉलम सहेजे जाते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | XLSX फ़ॉर्मेट में सहेजने के लिए व्यू कॉलम की सूची। ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) |

