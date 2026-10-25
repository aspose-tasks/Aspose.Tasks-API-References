---
title: "GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ग्राफ़िकल इंडिकेटर मानदंड की शर्त जाँच में उपयोग किए जाने वाले मान का प्रतिनिधित्व करता है।"
type: docs
weight: 117
url: /hi/java/com.aspose.tasks/graphicalindicatorcriteriavalue/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteriaValue
```

ग्राफ़िकल इंडिकेटर मानदंड की शर्त जाँच में उपयोग किए जाने वाले मान का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [GraphicalIndicatorCriteriaValue(BigDecimal value)](#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-) | GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर BigDecimal मान के साथ बनाता है। |
| [GraphicalIndicatorCriteriaValue(Date dateValue)](#GraphicalIndicatorCriteriaValue-java.util.Date-) | GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर Date मान के साथ बनाता है। |
| [GraphicalIndicatorCriteriaValue(String textValue)](#GraphicalIndicatorCriteriaValue-java.lang.String-) | GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर String मान के साथ बनाता है। |
| [GraphicalIndicatorCriteriaValue(Duration durationValue)](#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-) | GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर Duration मान के साथ बनाता है। |
| [GraphicalIndicatorCriteriaValue(boolean flagValue)](#GraphicalIndicatorCriteriaValue-boolean-) | GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर फ़्लैग (boolean) मान के साथ बनाता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [createFieldLink(int field)](#createFieldLink-int-) | GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस बनाता है जो निर्दिष्ट MS Project फ़ील्ड के मान को दर्शाता है। |
| [getRawValue()](#getRawValue--) | फ़ील्ड मान का अंतर्निहित स्थिर प्राप्त करता है। |
| [isFieldLink()](#isFieldLink--) | जाँचता है कि वर्तमान इंस्टेंस फ़ील्ड लिंक है (फ़ील्ड के मान को दर्शाता है) या नहीं। |
| [toString()](#toString--) | वर्तमान ऑब्जेक्ट का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है। |
### GraphicalIndicatorCriteriaValue(BigDecimal value) {#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-}
```
public GraphicalIndicatorCriteriaValue(BigDecimal value)
```


GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर BigDecimal मान के साथ बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | BigDecimal मान |

### GraphicalIndicatorCriteriaValue(Date dateValue) {#GraphicalIndicatorCriteriaValue-java.util.Date-}
```
public GraphicalIndicatorCriteriaValue(Date dateValue)
```


GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर Date मान के साथ बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dateValue | java.util.Date | Date मान |

### GraphicalIndicatorCriteriaValue(String textValue) {#GraphicalIndicatorCriteriaValue-java.lang.String-}
```
public GraphicalIndicatorCriteriaValue(String textValue)
```


GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर String मान के साथ बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| textValue | java.lang.String | String मान |

### GraphicalIndicatorCriteriaValue(Duration durationValue) {#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-}
```
public GraphicalIndicatorCriteriaValue(Duration durationValue)
```


GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर Duration मान के साथ बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | Duration मान |

### GraphicalIndicatorCriteriaValue(boolean flagValue) {#GraphicalIndicatorCriteriaValue-boolean-}
```
public GraphicalIndicatorCriteriaValue(boolean flagValue)
```


GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस स्थिर फ़्लैग (boolean) मान के साथ बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| flagValue | boolean | फ़्लैग (boolean) मान |

### createFieldLink(int field) {#createFieldLink-int-}
```
public static GraphicalIndicatorCriteriaValue createFieldLink(int field)
```


GraphicalIndicatorCriteriaValue क्लास का एक इंस्टेंस बनाता है जो निर्दिष्ट MS Project फ़ील्ड के मान को दर्शाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ील्ड | int | निर्दिष्ट फ़ील्ड |

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - instance of GraphicalIndicatorCriteriaValue class representing the value of the specified field
### getRawValue() {#getRawValue--}
```
public final Object getRawValue()
```


फ़ील्ड मान का अंतर्निहित स्थिर प्राप्त करता है।

**Returns:**
java.lang.Object - फ़ील्ड मान का मूल स्थिरांक
### isFieldLink() {#isFieldLink--}
```
public final boolean isFieldLink()
```


जाँचता है कि वर्तमान इंस्टेंस फ़ील्ड लिंक है (फ़ील्ड के मान को दर्शाता है) या नहीं।

**Returns:**
boolean - क्या वर्तमान इंस्टेंस एक फ़ील्ड लिंक है (फ़ील्ड के मान का प्रतिनिधित्व करता है)
### toString() {#toString--}
```
public String toString()
```


वर्तमान ऑब्जेक्ट का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है।

**Returns:**
java.lang.String - एक स्ट्रिंग जो वर्तमान ऑब्जेक्ट का प्रतिनिधित्व करती है
