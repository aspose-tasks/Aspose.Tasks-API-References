---
title: "AssignmentViewColumn"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट्स व्यू क्लास।"
type: docs
weight: 19
url: /hi/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

प्रोजेक्ट का व्यू क्लास।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | AssignmentViewColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | वर्तमान रिसोर्स असाइनमेंट को कॉलम टेक्स्ट में परिवर्तित करता है। |
| [getField()](#getField--) | कॉलम फ़ील्ड लौटाता है। |
| [setField(int value)](#setField-int-) | कॉलम फ़ील्ड सेट करता है। |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


AssignmentViewColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | कॉलम का नाम। |
| width | int | पिक्सेल में कॉलम की चौड़ाई। |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | असाइनमेंट डेटा को कॉलम टेक्स्ट में बदलने वाला कन्वर्टर। |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


वर्तमान रिसोर्स असाइनमेंट को कॉलम टेक्स्ट में परिवर्तित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | वर्तमान असाइनमेंट। |

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

