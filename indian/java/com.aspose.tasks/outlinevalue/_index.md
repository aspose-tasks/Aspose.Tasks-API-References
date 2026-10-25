---
title: "OutlineValue"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक आउटलाइन मान का प्रतिनिधित्व करता है।"
type: docs
weight: 173
url: /hi/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

एक आउटलाइन मान का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getDescription()](#getDescription--) | एक आउटलाइन वैल्यू का विवरण प्राप्त करता है। |
| [getDurationValue()](#getDurationValue--) | यदि प्रकार Duration है तो अवधि प्राप्त करता है। |
| [getParentValueId()](#getParentValueId--) | आउटलाइन कोड के पैरेंट नोड की Id प्राप्त करता है। |
| [getType()](#getType--) | आउटलाइन कोड प्रकार प्राप्त करता है। |
| [getValue()](#getValue--) | वास्तविक मान प्राप्त करता है। |
| [getValueGuid()](#getValueGuid--) | पूरे प्रोजेक्ट में इस मान को अन्य मानों में पहचानने वाला GUID प्राप्त करता है। |
| [getValueId()](#getValueId--) | परियोजना के भीतर एक आउटलाइन कोड वैल्यू की विशिष्ट Id प्राप्त करता है। |
| [isCollapsed()](#isCollapsed--) | एक मान प्राप्त करता है जो दर्शाता है कि आउटलाइन वैल्यू संकुचित है या नहीं। |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | एक मान सेट करता है जो दर्शाता है कि आउटलाइन वैल्यू संकुचित है या नहीं। |
| [setDescription(String value)](#setDescription-java.lang.String-) | एक आउटलाइन वैल्यू का विवरण सेट करता है। |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | यदि प्रकार Duration है तो अवधि सेट करता है। |
| [setParentValueId(int value)](#setParentValueId-int-) | आउटलाइन कोड के पैरेंट नोड की Id सेट करता है। |
| [setType(int value)](#setType-int-) | आउटलाइन कोड प्रकार सेट करता है। |
| [setValue(String value)](#setValue-java.lang.String-) | वास्तविक मान सेट करता है। |
| [setValueId(int value)](#setValueId-int-) | परियोजना के भीतर एक आउटलाइन कोड वैल्यू की विशिष्ट Id सेट करता है। |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


एक आउटलाइन वैल्यू का विवरण प्राप्त करता है।

**Returns:**
java.lang.String - एक आउटलाइन वैल्यू का विवरण।
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


यदि प्रकार Duration है तो अवधि प्राप्त करता है।

--------------------

जब आपको Duration प्रकार वाले OutlineValues के लिए मान सेट करने की आवश्यकता हो, तो इस प्रॉपर्टी को `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)) के ऊपर प्राथमिकता दें।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


आउटलाइन कोड के पैरेंट नोड की Id प्राप्त करता है।

**Returns:**
int - एक आउटलाइन कोड के पैरेंट नोड की Id।
### getType() {#getType--}
```
public final int getType()
```


आउटलाइन कोड प्रकार प्राप्त करता है।

**Returns:**
int - आउटलाइन कोड प्रकार।
### getValue() {#getValue--}
```
public final String getValue()
```


वास्तविक मान प्राप्त करता है।

**Returns:**
java.lang.String - वास्तविक मान।
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


पूरे प्रोजेक्ट में इस मान को अन्य मानों में पहचानने वाला GUID प्राप्त करता है।

**Returns:**
java.util.UUID - एक GUID जो पूरे प्रोजेक्ट में इस मान को अन्य मानों से पहचानता है।
### getValueId() {#getValueId--}
```
public final int getValueId()
```


परियोजना के भीतर एक आउटलाइन कोड वैल्यू की विशिष्ट Id प्राप्त करता है।

**Returns:**
int - परियोजना के भीतर एक आउटलाइन कोड वैल्यू की विशिष्ट Id।
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


एक मान प्राप्त करता है जो दर्शाता है कि आउटलाइन वैल्यू संकुचित है या नहीं।

--------------------

यह MS Project 2010 प्रॉपर्टी के लिए नया है।

**Returns:**
boolean - एक मान जो दर्शाता है कि आउटलाइन वैल्यू संकुचित है या नहीं।
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि आउटलाइन वैल्यू संकुचित है या नहीं।

--------------------

यह MS Project 2010 प्रॉपर्टी के लिए नया है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि रूपरेखा मान संकुचित है या नहीं. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


एक आउटलाइन वैल्यू का विवरण सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | रूपरेखा मान का विवरण. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


यदि प्रकार Duration है तो अवधि सेट करता है।

--------------------

जब आपको Duration प्रकार वाले OutlineValues के लिए मान सेट करने की आवश्यकता हो, तो इस प्रॉपर्टी को `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)) के ऊपर प्राथमिकता दें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | यदि प्रकार अवधि है तो अवधि. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


आउटलाइन कोड के पैरेंट नोड की Id सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | रूपरेखा कोड के पैरेंट नोड की आईडी. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


आउटलाइन कोड प्रकार सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | रूपरेखा कोड प्रकार. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


वास्तविक मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | वास्तविक मान. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


परियोजना के भीतर एक आउटलाइन कोड वैल्यू की विशिष्ट Id सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | परियोजना के भीतर रूपरेखा कोड मान की अद्वितीय आईडी. |

