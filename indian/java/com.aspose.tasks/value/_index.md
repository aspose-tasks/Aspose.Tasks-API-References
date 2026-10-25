---
title: "मान"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "मूल्य सूची में एक मान को दर्शाता है।"
type: docs
weight: 333
url: /hi/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

मूल्य सूची में एक मान को दर्शाता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Value()](#Value--) | नया उदाहरण प्रारंभ करता है [Value](../../com.aspose/tasks/value) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getDateValue()](#getDateValue--) | यदि इसे DateTime के रूप में दर्शाया जा सकता है तो वास्तविक मान प्राप्त करता है। |
| [getDescription()](#getDescription--) | किसी मान का विवरण प्राप्त करता है। |
| [getDuration()](#getDuration--) | Duration को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान प्राप्त करता है। |
| [getId()](#getId--) | परियोजना में किसी मान का अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [getNumericValue()](#getNumericValue--) | संख्या या लागत मान को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान प्राप्त करता है। |
| [getPhonetic()](#getPhonetic--) | कस्टम फ़ील्ड नाम के बारे में ध्वन्यात्मक जानकारी प्राप्त करता है। |
| [getStringValue()](#getStringValue--) | टेक्स्ट स्ट्रिंग को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान प्राप्त करता है। |
| [getVal()](#getVal--) | आंतरिक प्रतिनिधित्व में वास्तविक मान प्राप्त करता है। |
| [getValueGuid()](#getValueGuid--) | पूरे प्रोजेक्ट में इस मान को अन्य मानों में पहचानने वाला GUID प्राप्त करता है। |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | यदि इसे DateTime के रूप में दर्शाया जा सकता है तो वास्तविक मान सेट करता है। |
| [setDescription(String value)](#setDescription-java.lang.String-) | किसी मान का विवरण सेट करता है। |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Duration को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान सेट करता है। |
| [setId(int value)](#setId-int-) | परियोजना में किसी मान का अद्वितीय पहचानकर्ता सेट करता है। |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | संख्या या लागत मान को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान सेट करता है। |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | कस्टम फ़ील्ड नाम के बारे में ध्वन्यात्मक जानकारी सेट करता है। |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | टेक्स्ट स्ट्रिंग को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान सेट करता है। |
| [setVal(String value)](#setVal-java.lang.String-) | आंतरिक प्रतिनिधित्व में वास्तविक मान सेट करता है। |
### Value() {#Value--}
```
public Value()
```


नया उदाहरण प्रारंभ करता है [Value](../../com.aspose/tasks/value) क्लास का।

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


यदि इसे DateTime के रूप में दर्शाया जा सकता है तो वास्तविक मान प्राप्त करता है। डिफ़ॉल्ट मान है DateTime\#MinValue.MinValue।

--------------------

जब आपको DateTime मान सेट करना हो, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) की बजाय इस प्रॉपर्टी को प्राथमिकता दें।

**Returns:**
java.util.Date - वास्तविक मान यदि इसे DateTime के रूप में प्रस्तुत किया जा सकता है।
### getDescription() {#getDescription--}
```
public final String getDescription()
```


किसी मान का विवरण प्राप्त करता है।

**Returns:**
java.lang.String - किसी मान का विवरण।
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Duration को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान प्राप्त करता है।

--------------------

जब आपको Duration मान सेट करना हो, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) की बजाय इस प्रॉपर्टी को प्राथमिकता दें।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


परियोजना में किसी मान का अद्वितीय पहचानकर्ता प्राप्त करता है।

विभिन्न [Value](../../com.aspose.tasks/value) उदाहरणों के लिए समान पहचानकर्ता न रखने का महत्व है।

न्यूनतम `Id`([getId()](../../com.aspose/tasks/value\#getId--)/[setId(int)](../../com.aspose/tasks/value\#setId-int-)) मान `1` है।

**Returns:**
int - प्रोजेक्ट में किसी मान का अद्वितीय पहचानकर्ता।
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


संख्या या लागत मान को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान प्राप्त करता है।

--------------------

जब आपको Number या Cost मान सेट करना हो, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) की बजाय इस प्रॉपर्टी को प्राथमिकता दें।

**Returns:**
java.math.BigDecimal - वह वास्तविक मान जो संख्या या लागत मान को दर्शाने के लिए उपयोग किया जाता है।
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


कस्टम फ़ील्ड नाम के बारे में ध्वन्यात्मक जानकारी प्राप्त करता है।

**Returns:**
java.lang.String - कस्टम फ़ील्ड नाम के बारे में ध्वन्यात्मक जानकारी।
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


टेक्स्ट स्ट्रिंग को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान प्राप्त करता है।

--------------------

जब आपको Text मान सेट करना हो, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) की बजाय इस प्रॉपर्टी को प्राथमिकता दें।

**Returns:**
java.lang.String - वह वास्तविक मान जो टेक्स्ट स्ट्रिंग को दर्शाने के लिए उपयोग किया जाता है।
### getVal() {#getVal--}
```
public final String getVal()
```


आंतरिक प्रतिनिधित्व में वास्तविक मान प्राप्त करता है। नीचे सूचीबद्ध मजबूत टाइप वाली प्रॉपर्टी का उपयोग करने को प्राथमिकता दें।

--------------------

यदि आप Text मान सेट करना चाहते हैं तो मजबूत टाइप वाली `StringValue`([getStringValue()](../../com.aspose/tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose/tasks/value\#setStringValue-String-)) प्रॉपर्टी का उपयोग करने को प्राथमिकता दें।

यदि आप Number या Cost मान सेट करना चाहते हैं तो मजबूत टाइप वाली `NumericValue`([getNumericValue()](../../com.aspose/tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose/tasks/value\#setNumericValue-java.math.BigDecimal-)) प्रॉपर्टी का उपयोग करने को प्राथमिकता दें।

यदि आप Date/Start/Finish मान सेट करना चाहते हैं, तो मजबूत टाइप वाली `DateValue`([getDateValue()](../../com.aspose/tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose/tasks/value\#setDateValue-java.util.Date-)) प्रॉपर्टी का उपयोग करने को प्राथमिकता दें।

यदि आप Duration मान सेट करना चाहते हैं, तो मजबूत टाइप वाली `Duration`([getDuration()](../../com.aspose/tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/value\#setDuration-Duration-)) प्रॉपर्टी का उपयोग करने को प्राथमिकता दें।

यदि आपका प्रकार सूचीबद्ध नहीं है, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) प्रॉपर्टी का उपयोग करें।

**Returns:**
java.lang.String - आंतरिक प्रतिनिधित्व में वास्तविक मान।
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


पूरे प्रोजेक्ट में इस मान को अन्य मानों में पहचानने वाला GUID प्राप्त करता है।

**Returns:**
java.util.UUID - एक GUID जो पूरे प्रोजेक्ट में इस मान को अन्य मानों से पहचानता है।
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


यदि इसे DateTime के रूप में प्रस्तुत किया जा सकता है तो वास्तविक मान सेट करता है। डिफ़ॉल्ट मान DateTime\#MinValue.MinValue है।

--------------------

जब आपको DateTime मान सेट करना हो, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) की बजाय इस प्रॉपर्टी को प्राथमिकता दें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | वास्तविक मान यदि इसे DateTime के रूप में प्रस्तुत किया जा सकता है। |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


किसी मान का विवरण सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | किसी मान का विवरण। |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Duration को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान सेट करता है।

--------------------

जब आपको Duration मान सेट करना हो, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) की बजाय इस प्रॉपर्टी को प्राथमिकता दें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | वास्तविक मान जो Duration को दर्शाने के लिए उपयोग किया जाता है। |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


परियोजना में किसी मान का अद्वितीय पहचानकर्ता सेट करता है।

विभिन्न [Value](../../com.aspose.tasks/value) उदाहरणों के लिए समान पहचानकर्ता न रखने का महत्व है।

न्यूनतम `Id`([getId()](../../com.aspose/tasks/value\#getId--)/[setId(int)](../../com.aspose/tasks/value\#setId-int-)) मान `1` है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | परियोजना में किसी मान का अद्वितीय पहचानकर्ता। |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


संख्या या लागत मान को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान सेट करता है।

--------------------

जब आपको Number या Cost मान सेट करना हो, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) की बजाय इस प्रॉपर्टी को प्राथमिकता दें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | संख्या या लागत मान को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान। |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


कस्टम फ़ील्ड नाम के बारे में ध्वन्यात्मक जानकारी सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | कस्टम फ़ील्ड नाम के बारे में ध्वन्यात्मक जानकारी। |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


टेक्स्ट स्ट्रिंग को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान सेट करता है।

--------------------

जब आपको Text मान सेट करना हो, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) की बजाय इस प्रॉपर्टी को प्राथमिकता दें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | टेक्स्ट स्ट्रिंग को दर्शाने के लिए उपयोग किया जाने वाला वास्तविक मान। |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


आंतरिक प्रतिनिधित्व में वास्तविक मान सेट करता है। नीचे सूचीबद्ध सख्त टाइप्ड प्रॉपर्टीज़ का उपयोग करने को प्राथमिकता दें।

--------------------

यदि आप Text मान सेट करना चाहते हैं तो मजबूत टाइप वाली `StringValue`([getStringValue()](../../com.aspose/tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose/tasks/value\#setStringValue-String-)) प्रॉपर्टी का उपयोग करने को प्राथमिकता दें।

यदि आप Number या Cost मान सेट करना चाहते हैं तो मजबूत टाइप वाली `NumericValue`([getNumericValue()](../../com.aspose/tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose/tasks/value\#setNumericValue-java.math.BigDecimal-)) प्रॉपर्टी का उपयोग करने को प्राथमिकता दें।

यदि आप Date/Start/Finish मान सेट करना चाहते हैं, तो सख्त टाइप्ड `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) प्रॉपर्टी का उपयोग करने को प्राथमिकता दें।

यदि आप Duration मान सेट करना चाहते हैं, तो मजबूत टाइप वाली `Duration`([getDuration()](../../com.aspose/tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/value\#setDuration-Duration-)) प्रॉपर्टी का उपयोग करने को प्राथमिकता दें।

यदि आपका प्रकार सूचीबद्ध नहीं है, तो `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) प्रॉपर्टी का उपयोग करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | आंतरिक प्रतिनिधित्व में वास्तविक मान। |

