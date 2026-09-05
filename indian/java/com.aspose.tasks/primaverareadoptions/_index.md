---
title: "PrimaveraReadOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Primavera Xml या Primavera Xer फ़ाइलें पढ़ते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 206
url: /hi/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Primavera Xml या Primavera Xer फ़ाइलें पढ़ते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | एक नया उदाहरण प्रारंभ करता है [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि संस्थाओं के मूल अद्वितीय पहचानकर्ता संरक्षित किए जाने चाहिए या नहीं। |
| [getProjectUid()](#getProjectUid--) | एक प्रोजेक्ट का UID प्राप्त करता है जिसे कई प्रोजेक्ट्स वाली फ़ाइल से पढ़ा जाना है। |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि बेसलाइन प्रोजेक्ट्स लोड किए जाने चाहिए या नहीं। |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | XER फ़ॉर्मेट से पढ़े गए अपरिभाषित प्रतिबंधों वाले कार्यों को प्रोसेस करने के लिए उपयोग किए जाने वाले व्यवहार को निर्दिष्ट करता है। |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | एक फ़्लैग सेट करता है जो निर्धारित करता है कि संस्थाओं के मूल अद्वितीय पहचानकर्ता संरक्षित किए जाने चाहिए या नहीं। |
| [setProjectUid(int value)](#setProjectUid-int-) | कई प्रोजेक्ट्स वाली फ़ाइल से पढ़े जाने वाले प्रोजेक्ट का UID सेट करता है। |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | एक फ़्लैग सेट करता है जो निर्धारित करता है कि बेसलाइन प्रोजेक्ट्स लोड किए जाने चाहिए या नहीं। |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | XER फ़ॉर्मेट से पढ़े गए अपरिभाषित प्रतिबंधों वाले कार्यों को प्रोसेस करने के लिए उपयोग किए जाने वाले व्यवहार को निर्दिष्ट करता है। |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


एक नया उदाहरण प्रारंभ करता है [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) क्लास का।

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि संस्थाओं के मूल अद्वितीय पहचानकर्ता संरक्षित किए जाने चाहिए या नहीं।

**Returns:**
boolean - एक फ़्लैग जो निर्धारित करता है कि संस्थाओं के मूल अद्वितीय पहचानकर्ता संरक्षित किए जाने चाहिए या नहीं।
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


एक प्रोजेक्ट का UID प्राप्त करता है जिसे कई प्रोजेक्ट्स वाली फ़ाइल से पढ़ा जाना है।

**Returns:**
int - कई प्रोजेक्ट्स वाली फ़ाइल से पढ़े जाने वाले प्रोजेक्ट का UID।
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


एक फ़्लैग प्राप्त करता है जो निर्धारित करता है कि बेसलाइन प्रोजेक्ट्स लोड किए जाने चाहिए या नहीं। डिफ़ॉल्ट मान true है।

--------------------

यह फ़्लैग Primavera XML फ़ाइलों पर लागू होता है जिनमें बेसलाइन प्रोजेक्ट्स होते हैं (बेसलाइन XER फ़ॉर्मेट द्वारा समर्थित नहीं हैं)। जब बेसलाइन डेटा की आवश्यकता नहीं होती है, तो बड़े प्रोजेक्ट को तेज़ी से लोड करने के लिए इस विकल्प को false सेट किया जा सकता है।

**Returns:**
boolean - एक फ़्लैग जो निर्धारित करता है कि बेसलाइन प्रोजेक्ट्स लोड किए जाने चाहिए या नहीं।
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


XER फ़ॉर्मेट से पढ़े गए अपरिभाषित प्रतिबंधों वाले कार्यों को प्रोसेस करने के लिए उपयोग किए जाने वाले व्यवहार को निर्दिष्ट करता है।

**Returns:**
int - XER फ़ॉर्मेट से पढ़े गए अपरिभाषित प्रतिबंधों वाले कार्यों को प्रोसेस करने के लिए उपयोग किया गया व्यवहार।
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


एक फ़्लैग सेट करता है जो निर्धारित करता है कि संस्थाओं के मूल अद्वितीय पहचानकर्ता संरक्षित किए जाने चाहिए या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक फ़्लैग जो निर्धारित करता है कि संस्थाओं के मूल अद्वितीय पहचानकर्ता संरक्षित किए जाने चाहिए या नहीं। |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


कई प्रोजेक्ट्स वाली फ़ाइल से पढ़े जाने वाले प्रोजेक्ट का UID सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | कई प्रोजेक्ट्स वाली फ़ाइल से पढ़े जाने वाले प्रोजेक्ट का UID। |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


एक फ़्लैग सेट करता है जो निर्धारित करता है कि बेसलाइन प्रोजेक्ट्स लोड किए जाने चाहिए या नहीं। डिफ़ॉल्ट मान true है।

--------------------

यह फ़्लैग Primavera XML फ़ाइलों पर लागू होता है जिनमें बेसलाइन प्रोजेक्ट्स होते हैं (बेसलाइन XER फ़ॉर्मेट द्वारा समर्थित नहीं हैं)। जब बेसलाइन डेटा की आवश्यकता नहीं होती है, तो बड़े प्रोजेक्ट को तेज़ी से लोड करने के लिए इस विकल्प को false सेट किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक फ़्लैग जो निर्धारित करता है कि बेसलाइन प्रोजेक्ट्स लोड किए जाने चाहिए या नहीं। |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


XER फ़ॉर्मेट से पढ़े गए अपरिभाषित प्रतिबंधों वाले कार्यों को प्रोसेस करने के लिए उपयोग किए जाने वाले व्यवहार को निर्दिष्ट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | XER फ़ॉर्मेट से पढ़े गए अपरिभाषित प्रतिबंधों वाले कार्यों को प्रोसेस करने के लिए उपयोग किया जाने वाला व्यवहार। |

