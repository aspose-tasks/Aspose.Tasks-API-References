---
title: "OleObject"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक OLE ऑब्जेक्ट का प्रतिनिधित्व करता है जिसे MPP फ़ाइल के गैंट चार्ट दृश्य में सम्मिलित किया जा सकता है।"
type: docs
weight: 164
url: /hi/java/com.aspose.tasks/oleobject/
---

**Inheritance:**
java.lang.Object
```
public class OleObject
```

एक OLE ऑब्जेक्ट का प्रतिनिधित्व करता है जिसे MPP फ़ाइल के गैंट चार्ट दृश्य में सम्मिलित किया जा सकता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [OleObject()](#OleObject--) | नए [OleObject](../../com.aspose.tasks/oleobject) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getApplicationName()](#getApplicationName--) | एम्बेडेड ऑब्जेक्ट खोलने के लिए एप्लिकेशन का नाम प्राप्त करता है। |
| [getContent()](#getContent--) | एम्बेडेड फ़ाइल का डेटा प्राप्त करता है; यदि कोई डेटा एम्बेड नहीं किया गया हो तो null। |
| [getDisplayAsIcon()](#getDisplayAsIcon--) | एक फ़्लैग प्राप्त करता है जो दर्शाता है कि OLE ऑब्जेक्ट को आइकन के रूप में या उसकी सामान्य तस्वीर के रूप में दिखाया जाना चाहिए। |
| [getFileFormat()](#getFileFormat--) | एम्बेडेड ऑब्जेक्ट का फ़ाइल फ़ॉर्मेट प्राप्त करता है। |
| [getFullPath()](#getFullPath--) | डालें गए ऑब्जेक्ट का पूर्ण पाथ प्राप्त करता है। |
| [getId()](#getId--) | ऑब्जेक्ट आईडी प्राप्त करता है। |
| [getLabel()](#getLabel--) | डालें गए ऑब्जेक्ट का लेबल प्राप्त करता है। |
| [getLinked()](#getLinked--) | एक मान प्राप्त करता है जो दर्शाता है कि प्रोजेक्ट फ़ाइल में केवल लिंक स्रोत पर संग्रहीत वास्तविक डेटा का लिंक ही है या नहीं। |
| [getName()](#getName--) | OLE ऑब्जेक्ट के इंस्टेंस का नाम प्राप्त करता है। |
| [getTemporaryFile()](#getTemporaryFile--) | डालें गए ऑब्जेक्ट की अस्थायी फ़ाइल का पाथ प्राप्त करता है। |
| [getView()](#getView--) | डालें गए ऑब्जेक्ट से संबंधित `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) क्लास का इंस्टेंस प्राप्त करता है। |
| [setApplicationName(String value)](#setApplicationName-java.lang.String-) | एम्बेडेड ऑब्जेक्ट खोलने के लिए एप्लिकेशन का नाम सेट करता है। |
| [setContent(byte[] value)](#setContent-byte---) | एम्बेडेड फ़ाइल का डेटा सेट करता है; यदि कोई डेटा एम्बेड नहीं किया गया हो तो null। |
| [setDisplayAsIcon(boolean value)](#setDisplayAsIcon-boolean-) | एक फ़्लैग सेट करता है जो दर्शाता है कि OLE ऑब्जेक्ट को आइकन के रूप में या उसकी सामान्य तस्वीर के रूप में दिखाया जाना चाहिए। |
| [setFileFormat(String value)](#setFileFormat-java.lang.String-) | एम्बेडेड ऑब्जेक्ट का फ़ाइल फ़ॉर्मेट सेट करता है। |
| [setFullPath(String value)](#setFullPath-java.lang.String-) | डालें गए ऑब्जेक्ट का पूर्ण पाथ सेट करता है। |
| [setId(int value)](#setId-int-) | ऑब्जेक्ट आईडी सेट करता है। |
| [setLabel(String value)](#setLabel-java.lang.String-) | डालें गए ऑब्जेक्ट का लेबल सेट करता है। |
| [setName(String value)](#setName-java.lang.String-) | OLE ऑब्जेक्ट की इंस्टेंस का नाम सेट करता है। |
| [setTemporaryFile(String value)](#setTemporaryFile-java.lang.String-) | डाली गई ऑब्जेक्ट की अस्थायी फ़ाइल का पथ सेट करता है। |
| [setView(View value)](#setView-com.aspose.tasks.View-) | डाली गई ऑब्जेक्ट जिस `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) क्लास से संबंधित है, उसकी इंस्टेंस सेट करता है। |
### OleObject() {#OleObject--}
```
public OleObject()
```


नए [OleObject](../../com.aspose.tasks/oleobject) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

### getApplicationName() {#getApplicationName--}
```
public final String getApplicationName()
```


एम्बेडेड ऑब्जेक्ट खोलने के लिए एप्लिकेशन का नाम प्राप्त करता है।

**Returns:**
java.lang.String - एम्बेडेड ऑब्जेक्ट को खोलने के लिए एप्लिकेशन का नाम।
### getContent() {#getContent--}
```
public final byte[] getContent()
```


एम्बेडेड फ़ाइल का डेटा प्राप्त करता है; यदि कोई डेटा एम्बेड नहीं किया गया हो तो null।

**Returns:**
byte[] - एम्बेडेड फ़ाइल का डेटा; यदि कोई डेटा एम्बेड नहीं किया गया तो null।
### getDisplayAsIcon() {#getDisplayAsIcon--}
```
public final boolean getDisplayAsIcon()
```


एक फ़्लैग प्राप्त करता है जो दर्शाता है कि OLE ऑब्जेक्ट को आइकन के रूप में या उसकी सामान्य तस्वीर के रूप में दिखाया जाना चाहिए।

**Returns:**
boolean - एक फ़्लैग जो दर्शाता है कि OLE ऑब्जेक्ट को आइकन के रूप में या उसकी सामान्य तस्वीर के रूप में दिखाया जाना चाहिए।
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


एम्बेडेड ऑब्जेक्ट का फ़ाइल फ़ॉर्मेट प्राप्त करता है।

**Returns:**
java.lang.String - एम्बेडेड ऑब्जेक्ट का फ़ाइल फ़ॉर्मेट।
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


डालें गए ऑब्जेक्ट का पूर्ण पाथ प्राप्त करता है।

**Returns:**
java.lang.String - डाली गई ऑब्जेक्ट का पूर्ण पथ।
### getId() {#getId--}
```
public final int getId()
```


ऑब्जेक्ट आईडी प्राप्त करता है।

**Returns:**
int - ऑब्जेक्ट आईडी।
### getLabel() {#getLabel--}
```
public final String getLabel()
```


डालें गए ऑब्जेक्ट का लेबल प्राप्त करता है।

**Returns:**
java.lang.String - डाली गई ऑब्जेक्ट का लेबल।
### getLinked() {#getLinked--}
```
public final boolean getLinked()
```


एक मान प्राप्त करता है जो दर्शाता है कि प्रोजेक्ट फ़ाइल में केवल लिंक स्रोत पर संग्रहीत वास्तविक डेटा का लिंक ही है या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि प्रोजेक्ट फ़ाइल में केवल लिंक स्रोत पर संग्रहीत वास्तविक डेटा का लिंक है या नहीं।
### getName() {#getName--}
```
public final String getName()
```


OLE ऑब्जेक्ट के इंस्टेंस का नाम प्राप्त करता है।

**Returns:**
java.lang.String - OLE ऑब्जेक्ट की इंस्टेंस का नाम।
### getTemporaryFile() {#getTemporaryFile--}
```
public final String getTemporaryFile()
```


डालें गए ऑब्जेक्ट की अस्थायी फ़ाइल का पाथ प्राप्त करता है।

**Returns:**
java.lang.String - डाली गई ऑब्जेक्ट की अस्थायी फ़ाइल का पथ।
### getView() {#getView--}
```
public final View getView()
```


डालें गए ऑब्जेक्ट से संबंधित `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) क्लास का इंस्टेंस प्राप्त करता है।

**Returns:**
[View](../../com.aspose.tasks/view) - the instance of the `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) class the inserted object belongs to.
### setApplicationName(String value) {#setApplicationName-java.lang.String-}
```
public final void setApplicationName(String value)
```


एम्बेडेड ऑब्जेक्ट खोलने के लिए एप्लिकेशन का नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | एम्बेडेड ऑब्जेक्ट को खोलने के लिए एप्लिकेशन का नाम। |

### setContent(byte[] value) {#setContent-byte---}
```
public final void setContent(byte[] value)
```


एम्बेडेड फ़ाइल का डेटा सेट करता है; यदि कोई डेटा एम्बेड नहीं किया गया हो तो null।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | byte[] | एम्बेडेड फ़ाइल का डेटा; यदि कोई डेटा एम्बेड नहीं किया गया तो null। |

### setDisplayAsIcon(boolean value) {#setDisplayAsIcon-boolean-}
```
public final void setDisplayAsIcon(boolean value)
```


एक फ़्लैग सेट करता है जो दर्शाता है कि OLE ऑब्जेक्ट को आइकन के रूप में या उसकी सामान्य तस्वीर के रूप में दिखाया जाना चाहिए।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक फ़्लैग जो दर्शाता है कि OLE ऑब्जेक्ट को आइकन के रूप में या उसकी सामान्य तस्वीर के रूप में दिखाया जाना चाहिए। |

### setFileFormat(String value) {#setFileFormat-java.lang.String-}
```
public final void setFileFormat(String value)
```


एम्बेडेड ऑब्जेक्ट का फ़ाइल फ़ॉर्मेट सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | एम्बेडेड ऑब्जेक्ट का फ़ाइल फ़ॉर्मेट। |

### setFullPath(String value) {#setFullPath-java.lang.String-}
```
public final void setFullPath(String value)
```


डालें गए ऑब्जेक्ट का पूर्ण पाथ सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | डाली गई ऑब्जेक्ट का पूर्ण पथ। |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


ऑब्जेक्ट आईडी सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | ऑब्जेक्ट आईडी। |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


डालें गए ऑब्जेक्ट का लेबल सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | डाली गई ऑब्जेक्ट का लेबल। |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


OLE ऑब्जेक्ट की इंस्टेंस का नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | OLE ऑब्जेक्ट की इंस्टेंस का नाम। |

### setTemporaryFile(String value) {#setTemporaryFile-java.lang.String-}
```
public final void setTemporaryFile(String value)
```


डाली गई ऑब्जेक्ट की अस्थायी फ़ाइल का पथ सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | डाली गई ऑब्जेक्ट की अस्थायी फ़ाइल का पथ। |

### setView(View value) {#setView-com.aspose.tasks.View-}
```
public final void setView(View value)
```


डाली गई ऑब्जेक्ट जिस `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) क्लास से संबंधित है, उसकी इंस्टेंस सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | डाली गई ऑब्जेक्ट जिस `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) क्लास से संबंधित है, उसकी इंस्टेंस। |

