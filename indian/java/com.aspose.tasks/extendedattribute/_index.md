---
title: "ExtendedAttribute"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "विस्तारित विशेषताओं को दर्शाता है।"
type: docs
weight: 81
url: /hi/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

विस्तारित विशेषताओं को दर्शाता है।

--------------------

वर्तमान में MSP Xml 2003/2007 और mpp 2003 से Extended attributes पढ़ने के सभी प्रकार समर्थित हैं। MSP mpp 2007 के लिए सभी Extended attributes पढ़ना समर्थित है, सिवाय अवधि और फ़्लैग्स के।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | एट्रिब्यूट परिभाषा प्राप्त करता है। |
| [getDateValue()](#getDateValue--) | तारीख प्रकार (Date, Start, Finish) वाले एट्रिब्यूट्स के लिए मान प्राप्त करता है। |
| [getDurationValue()](#getDurationValue--) | ‘Duration’ प्रकार के गुणों के लिए मान प्राप्त करता है। |
| [getFieldId()](#getFieldId--) | फ़ील्ड की आईडी प्राप्त करता है। |
| [getFlagValue()](#getFlagValue--) | ‘Flag’ प्रकार के गुण के लिए फ़्लैग सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getNumericValue()](#getNumericValue--) | संख्यात्मक प्रकार (Cost, Number) वाले गुणों के लिए मान प्राप्त करता है। |
| [getTextValue()](#getTextValue--) | ‘Text’ प्रकार के गुणों के लिए मान प्राप्त करता है। |
| [getValueGuid()](#getValueGuid--) | लुकअप मान का GUID प्राप्त करता है। |
| [getValueReadOnly()](#getValueReadOnly--) | इस [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) उदाहरण का मान केवल‑पढ़ने योग्य है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [isErrorValue()](#isErrorValue--) | विस्तारित गुण के मान की गणना में त्रुटि हुई है या नहीं, यह प्राप्त करता है। |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | तारीख प्रकार (Date, Start, Finish) वाले गुणों के लिए मान सेट करता है। |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | ‘Duration’ प्रकार के गुणों के लिए मान सेट करता है। |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | ‘Flag’ प्रकार के गुण के लिए फ़्लैग सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | संख्यात्मक प्रकार (Cost, Number) वाले गुणों के लिए मान सेट करता है। |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | ‘Text’ प्रकार के गुणों के लिए मान सेट करता है। |
| [toString()](#toString--) | विस्तारित गुण का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है। |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


एट्रिब्यूट परिभाषा प्राप्त करता है।

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


तारीख प्रकार (Date, Start, Finish) वाले एट्रिब्यूट्स के लिए मान प्राप्त करता है।

**Returns:**
java.util.Date - तारीख प्रकार (Date, Start, Finish) वाले गुणों के लिए मान।
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


‘Duration’ प्रकार के गुणों के लिए मान प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


फ़ील्ड की आईडी प्राप्त करता है।

**Returns:**
java.lang.String - फ़ील्ड की आईडी।
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


‘Flag’ प्रकार के गुण के लिए फ़्लैग सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - ‘Flag’ प्रकार के गुण के लिए फ़्लैग सेट है या नहीं, यह दर्शाने वाला मान।
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


संख्यात्मक प्रकार (Cost, Number) वाले गुणों के लिए मान प्राप्त करता है।

**Returns:**
java.math.BigDecimal - संख्यात्मक प्रकार (Cost, Number) वाले गुणों के लिए मान।
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


‘Text’ प्रकार के गुणों के लिए मान प्राप्त करता है।

**Returns:**
java.lang.String - ‘Text’ प्रकार के गुणों के लिए मान।
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


लुकअप मान का GUID प्राप्त करता है।

--------------------

इसे सीधे सेट नहीं करना चाहिए, बल्कि लुकअप मान के साथ एक विस्तारित गुण बनाने के लिए ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) का उपयोग करें।

**Returns:**
java.lang.String - लुकअप मान का GUID।
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


इस [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) उदाहरण का मान केवल‑पढ़ने योग्य है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

Value: यदि इस ऑब्जेक्ट के लिए [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) में कोई सूत्र या रोलअप परिभाषित है तो true लौटाता है।

**Returns:**
boolean - इस [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) उदाहरण का मान केवल‑पढ़ने योग्य है या नहीं, यह दर्शाने वाला मान।
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


विस्तारित गुण के मान की गणना में त्रुटि हुई है या नहीं, यह प्राप्त करता है।

**Returns:**
boolean - विस्तारित गुण के मान की गणना में त्रुटि हुई है या नहीं।
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


तारीख प्रकार (Date, Start, Finish) वाले गुणों के लिए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | तारीख प्रकार (Date, Start, Finish) वाले गुणों के लिए मान। |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


‘Duration’ प्रकार के गुणों के लिए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ‘Duration’ प्रकार वाले गुणों के लिए मान। |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


‘Flag’ प्रकार के गुण के लिए फ़्लैग सेट है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | ‘Flag’ प्रकार वाले गुण के लिए फ़्लैग सेट है या नहीं दर्शाने वाला मान। |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


संख्यात्मक प्रकार (Cost, Number) वाले गुणों के लिए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | संख्यात्मक प्रकार (Cost, Number) वाले गुणों के लिए मान। |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


‘Text’ प्रकार के गुणों के लिए मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | ‘Text’ प्रकार वाले गुणों के लिए मान। |

### toString() {#toString--}
```
public String toString()
```


विस्तारित गुण का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है।

**Returns:**
java.lang.String - विस्तारित गुण का स्ट्रिंग प्रतिनिधित्व।
