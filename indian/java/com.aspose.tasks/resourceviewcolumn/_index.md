---
title: "ResourceViewColumn"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ResourceUsage दृश्य और ResourceSheet दृश्य में उपयोग की जाने वाली Projects view क्लास।"
type: docs
weight: 261
url: /hi/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

परियोजना का दृश्य क्लास जो ResourceUsage दृश्य और ResourceSheet दृश्य में उपयोग किया जाता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | नया उदाहरण प्रारंभ करता है [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) क्लास का। |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | नया उदाहरण प्रारंभ करता है [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) क्लास का। |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | नया उदाहरण प्रारंभ करता है [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | वर्तमान संसाधन को कॉलम टेक्स्ट में परिवर्तित करता है। |
| [getField()](#getField--) | कॉलम फ़ील्ड लौटाता है। |
| [setField(int value)](#setField-int-) | कॉलम फ़ील्ड सेट करता है। |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


नया उदाहरण प्रारंभ करता है [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | कॉलम का नाम। |
| width | int | पिक्सेल में कॉलम की चौड़ाई। |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | संसाधन डेटा को कॉलम टेक्स्ट में परिवर्तित करने वाला कनवर्टर। |
| फ़ील्ड | int | कॉलम फ़ील्ड। |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


नया उदाहरण प्रारंभ करता है [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | कॉलम का नाम। |
| width | int | पिक्सेल में कॉलम की चौड़ाई। |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | संसाधन डेटा को कॉलम टेक्स्ट में परिवर्तित करने वाला कनवर्टर। |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


नया उदाहरण प्रारंभ करता है [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| width | int | पिक्सेल में कॉलम की चौड़ाई। |
| फ़ील्ड | int | कॉलम फ़ील्ड। |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


वर्तमान संसाधन को कॉलम टेक्स्ट में परिवर्तित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | वर्तमान संसाधन। |

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

