---
title: "OutlineCodeDefinition"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक आउटलाइन कोड परिभाषा का प्रतिनिधित्व करता है।"
type: docs
weight: 169
url: /hi/java/com.aspose.tasks/outlinecodedefinition/
---

**Inheritance:**
java.lang.Object
```
public final class OutlineCodeDefinition
```

एक आउटलाइन कोड परिभाषा का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [OutlineCodeDefinition()](#OutlineCodeDefinition--) | नए उदाहरण को प्रारंभ करता है [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) क्लास। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getAlias()](#getAlias--) | कस्टम आउटलाइन कोड का उपनाम प्राप्त करता है। |
| [getAllLevelsRequired()](#getAllLevelsRequired--) | एक मान प्राप्त करता है जो दर्शाता है कि नए कोड को सभी स्तरों की आवश्यकता है या नहीं। |
| [getEnterprise()](#getEnterprise--) | एक मान प्राप्त करता है जो दर्शाता है कि कस्टम आउटलाइन कोड एंटरप्राइज़ कस्टम आउटलाइन कोड है या नहीं। |
| [getEnterpriseOutlineCodeAlias()](#getEnterpriseOutlineCodeAlias--) | एक अन्य कस्टम फ़ील्ड का संदर्भ प्राप्त करता है जिसके लिए यह आउटलाइन कोड परिभाषा उपनाम है। |
| [getFieldId()](#getFieldId--) | आउटलाइन कोड का फ़ील्ड नंबर प्राप्त करता है। |
| [getFieldName()](#getFieldName--) | कस्टम आउटलाइन कोड का नाम प्राप्त करता है। |
| [getGuid()](#getGuid--) | आउटलाइन कोड का GUID प्राप्त करता है। |
| [getLeafOnly()](#getLeafOnly--) | एक मान प्राप्त करता है जो दर्शाता है कि इस आउटलाइन कोड फ़ील्ड में निर्दिष्ट मान लीफ़ वैल्यू होने चाहिए या नहीं। |
| [getMasks()](#getMasks--) | OutlineMaskCollection ऑब्जेक्ट प्राप्त करता है। |
| [getOnlyTableValuesAllowed()](#getOnlyTableValuesAllowed--) | एक मान प्राप्त करता है जो दर्शाता है कि निर्दिष्ट मान मान तालिका से आने चाहिए या नहीं। |
| [getPhoneticAlias()](#getPhoneticAlias--) | कस्टम आउटलाइन कोड के उपनाम का ध्वन्यात्मक उच्चारण प्राप्त करता है। |
| [getResourceSubstitutionEnabled()](#getResourceSubstitutionEnabled--) | एक मान प्राप्त करता है जो दर्शाता है कि कस्टम आउटलाइन कोड को माइक्रोसॉफ्ट प्रोजेक्ट में रिसोर्स सब्स्टिट्यूशन विज़ार्ड द्वारा उपयोग किया जा सकता है या नहीं। |
| [getShowIndent()](#getShowIndent--) | एक मान प्राप्त करता है जो दर्शाता है कि इस आउटलाइन कोड के इंडेंट दिखाए जाने चाहिए या नहीं। |
| [getValues()](#getValues--) | OutlineValueCollection ऑब्जेक्ट प्राप्त करता है। |
| [setAlias(String value)](#setAlias-java.lang.String-) | कस्टम आउटलाइन कोड का उपनाम सेट करता है। |
| [setAllLevelsRequired(boolean value)](#setAllLevelsRequired-boolean-) | एक मान सेट करता है जो दर्शाता है कि नए कोड को सभी स्तरों की आवश्यकता है या नहीं। |
| [setEnterprise(boolean value)](#setEnterprise-boolean-) | एक मान सेट करता है जो दर्शाता है कि कस्टम आउटलाइन कोड एंटरप्राइज़ कस्टम आउटलाइन कोड है या नहीं। |
| [setEnterpriseOutlineCodeAlias(int value)](#setEnterpriseOutlineCodeAlias-int-) | एक अन्य कस्टम फ़ील्ड का संदर्भ सेट करता है जिसके लिए यह आउटलाइन कोड परिभाषा उपनाम है। |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | आउटलाइन कोड का फ़ील्ड नंबर सेट करता है। |
| [setFieldName(String value)](#setFieldName-java.lang.String-) | कस्टम आउटलाइन कोड का नाम सेट करता है। |
| [setGuid(String value)](#setGuid-java.lang.String-) | आउटलाइन कोड का GUID सेट करता है। |
| [setLeafOnly(boolean value)](#setLeafOnly-boolean-) | एक मान सेट करता है जो दर्शाता है कि इस आउटलाइन कोड फ़ील्ड में निर्दिष्ट मान लीफ़ वैल्यू होने चाहिए या नहीं। |
| [setOnlyTableValuesAllowed(boolean value)](#setOnlyTableValuesAllowed-boolean-) | एक मान सेट करता है जो यह दर्शाता है कि निर्दिष्ट मानों को मान तालिका से आना चाहिए। |
| [setPhoneticAlias(String value)](#setPhoneticAlias-java.lang.String-) | कस्टम आउटलाइन कोड के उपनाम की ध्वन्यात्मक उच्चारण सेट करता है। |
| [setResourceSubstitutionEnabled(boolean value)](#setResourceSubstitutionEnabled-boolean-) | एक मान सेट करता है जो यह दर्शाता है कि कस्टम आउटलाइन कोड को Microsoft Project में रिसोर्स सब्स्टिट्यूशन विज़ार्ड द्वारा उपयोग किया जा सकता है या नहीं। |
| [setShowIndent(boolean value)](#setShowIndent-boolean-) | एक मान सेट करता है जो यह दर्शाता है कि इस आउटलाइन कोड के इंडेंट दिखाए जाने चाहिए या नहीं। |
### OutlineCodeDefinition() {#OutlineCodeDefinition--}
```
public OutlineCodeDefinition()
```


नए उदाहरण को प्रारंभ करता है [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) क्लास।

### getAlias() {#getAlias--}
```
public final String getAlias()
```


कस्टम आउटलाइन कोड का उपनाम प्राप्त करता है।

**Returns:**
java.lang.String - एक कस्टम आउटलाइन कोड का उपनाम।
### getAllLevelsRequired() {#getAllLevelsRequired--}
```
public final boolean getAllLevelsRequired()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि नए कोड्स में सभी स्तर होने चाहिए या नहीं। एंटरप्राइज़ कोड्स के लिए उपलब्ध नहीं है।

**Returns:**
boolean - एक मान जो यह दर्शाता है कि नए कोड्स में सभी स्तर होने चाहिए या नहीं।
### getEnterprise() {#getEnterprise--}
```
public final boolean getEnterprise()
```


एक मान प्राप्त करता है जो दर्शाता है कि कस्टम आउटलाइन कोड एंटरप्राइज़ कस्टम आउटलाइन कोड है या नहीं।

**Returns:**
boolean - एक मान जो यह दर्शाता है कि एक कस्टम आउटलाइन कोड एंटरप्राइज़ कस्टम आउटलाइन कोड है या नहीं।
### getEnterpriseOutlineCodeAlias() {#getEnterpriseOutlineCodeAlias--}
```
public final int getEnterpriseOutlineCodeAlias()
```


एक अन्य कस्टम फ़ील्ड का संदर्भ प्राप्त करता है जिसके लिए यह आउटलाइन कोड परिभाषा उपनाम है।

**Returns:**
int - एक संदर्भ जो किसी अन्य कस्टम फ़ील्ड की ओर इशारा करता है जिसके लिए यह आउटलाइन कोड परिभाषा एक उपनाम है।
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


आउटलाइन कोड का फ़ील्ड नंबर प्राप्त करता है।

**Returns:**
java.lang.String - एक आउटलाइन कोड का फ़ील्ड नंबर।
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


कस्टम आउटलाइन कोड का नाम प्राप्त करता है।

**Returns:**
java.lang.String - एक कस्टम आउटलाइन कोड का नाम।
### getGuid() {#getGuid--}
```
public final String getGuid()
```


आउटलाइन कोड का GUID प्राप्त करता है।

**Returns:**
java.lang.String - एक आउटलाइन कोड का GUID।
### getLeafOnly() {#getLeafOnly--}
```
public final boolean getLeafOnly()
```


एक मान प्राप्त करता है जो दर्शाता है कि इस आउटलाइन कोड फ़ील्ड में निर्दिष्ट मान लीफ़ वैल्यू होने चाहिए या नहीं।

**Returns:**
boolean - एक मान जो यह दर्शाता है कि इस आउटलाइन कोड फ़ील्ड में निर्दिष्ट मानों को लीफ़ वैल्यू होना चाहिए या नहीं।
### getMasks() {#getMasks--}
```
public final OutlineMaskCollection getMasks()
```


OutlineMaskCollection ऑब्जेक्ट प्राप्त करता है। एंट्रीज़ की तालिका जो आउटलाइन कोड मास्क को परिभाषित करती है। केवल-रीड [OutlineMaskCollection](../../com.aspose.tasks/outlinemaskcollection) इंस्टेंस।

**Returns:**
[OutlineMaskCollection](../../com.aspose.tasks/outlinemaskcollection) - the OutlineMaskCollection object.
### getOnlyTableValuesAllowed() {#getOnlyTableValuesAllowed--}
```
public final boolean getOnlyTableValuesAllowed()
```


एक मान प्राप्त करता है जो दर्शाता है कि निर्दिष्ट मान मान तालिका से आने चाहिए या नहीं।

**Returns:**
boolean - एक मान जो यह दर्शाता है कि निर्दिष्ट मानों को मान तालिका से आना चाहिए या नहीं।
### getPhoneticAlias() {#getPhoneticAlias--}
```
public final String getPhoneticAlias()
```


कस्टम आउटलाइन कोड के उपनाम का ध्वन्यात्मक उच्चारण प्राप्त करता है।

**Returns:**
java.lang.String - कस्टम आउटलाइन कोड के उपनाम की ध्वन्यात्मक उच्चारण।
### getResourceSubstitutionEnabled() {#getResourceSubstitutionEnabled--}
```
public final boolean getResourceSubstitutionEnabled()
```


एक मान प्राप्त करता है जो दर्शाता है कि कस्टम आउटलाइन कोड को माइक्रोसॉफ्ट प्रोजेक्ट में रिसोर्स सब्स्टिट्यूशन विज़ार्ड द्वारा उपयोग किया जा सकता है या नहीं।

**Returns:**
boolean - एक मान जो यह दर्शाता है कि कस्टम आउटलाइन कोड को Microsoft Project में रिसोर्स सब्स्टिट्यूशन विज़ार्ड द्वारा उपयोग किया जा सकता है या नहीं।
### getShowIndent() {#getShowIndent--}
```
public final boolean getShowIndent()
```


एक मान प्राप्त करता है जो दर्शाता है कि इस आउटलाइन कोड के इंडेंट दिखाए जाने चाहिए या नहीं।

--------------------

यह MS Project 2010 प्रॉपर्टी के लिए नया है।

**Returns:**
boolean - एक मान जो यह दर्शाता है कि इस आउटलाइन कोड के इंडेंट दिखाए जाने चाहिए या नहीं।
### getValues() {#getValues--}
```
public final OutlineValueCollection getValues()
```


OutlineValueCollection ऑब्जेक्ट प्राप्त करता है। इस आउटलाइन कोड से संबंधित तालिका के मान।

**Returns:**
[OutlineValueCollection](../../com.aspose.tasks/outlinevaluecollection) - OutlineValueCollection object.
### setAlias(String value) {#setAlias-java.lang.String-}
```
public final void setAlias(String value)
```


कस्टम आउटलाइन कोड का उपनाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | एक कस्टम आउटलाइन कोड का उपनाम। |

### setAllLevelsRequired(boolean value) {#setAllLevelsRequired-boolean-}
```
public final void setAllLevelsRequired(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि नए कोड्स में सभी स्तर होने चाहिए या नहीं। एंटरप्राइज़ कोड्स के लिए उपलब्ध नहीं है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो यह दर्शाता है कि नए कोड्स में सभी स्तर होने चाहिए या नहीं। |

### setEnterprise(boolean value) {#setEnterprise-boolean-}
```
public final void setEnterprise(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि कस्टम आउटलाइन कोड एंटरप्राइज़ कस्टम आउटलाइन कोड है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो यह दर्शाता है कि एक कस्टम आउटलाइन कोड एंटरप्राइज़ कस्टम आउटलाइन कोड है या नहीं। |

### setEnterpriseOutlineCodeAlias(int value) {#setEnterpriseOutlineCodeAlias-int-}
```
public final void setEnterpriseOutlineCodeAlias(int value)
```


एक अन्य कस्टम फ़ील्ड का संदर्भ सेट करता है जिसके लिए यह आउटलाइन कोड परिभाषा उपनाम है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक संदर्भ जो किसी अन्य कस्टम फ़ील्ड की ओर इशारा करता है जिसके लिए यह आउटलाइन कोड परिभाषा एक उपनाम है। |

### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


आउटलाइन कोड का फ़ील्ड नंबर सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | एक आउटलाइन कोड का फ़ील्ड नंबर। |

### setFieldName(String value) {#setFieldName-java.lang.String-}
```
public final void setFieldName(String value)
```


कस्टम आउटलाइन कोड का नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | कस्टम आउटलाइन कोड का नाम। |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


आउटलाइन कोड का GUID सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | आउटलाइन कोड का Guid। |

### setLeafOnly(boolean value) {#setLeafOnly-boolean-}
```
public final void setLeafOnly(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि इस आउटलाइन कोड फ़ील्ड में निर्दिष्ट मान लीफ़ वैल्यू होने चाहिए या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि इस आउटलाइन कोड फ़ील्ड में निर्दिष्ट मानों को लीफ़ मान होना चाहिए या नहीं। |

### setOnlyTableValuesAllowed(boolean value) {#setOnlyTableValuesAllowed-boolean-}
```
public final void setOnlyTableValuesAllowed(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि निर्दिष्ट मानों को मान तालिका से आना चाहिए।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि निर्दिष्ट मानों को वैल्यूज़ टेबल से आना चाहिए या नहीं। |

### setPhoneticAlias(String value) {#setPhoneticAlias-java.lang.String-}
```
public final void setPhoneticAlias(String value)
```


कस्टम आउटलाइन कोड के उपनाम की ध्वन्यात्मक उच्चारण सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | कस्टम आउटलाइन कोड के उपनाम का ध्वन्यात्मक उच्चारण। |

### setResourceSubstitutionEnabled(boolean value) {#setResourceSubstitutionEnabled-boolean-}
```
public final void setResourceSubstitutionEnabled(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि कस्टम आउटलाइन कोड को Microsoft Project में रिसोर्स सब्स्टिट्यूशन विज़ार्ड द्वारा उपयोग किया जा सकता है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि कस्टम आउटलाइन कोड को Microsoft Project में रिसोर्स सब्स्टिट्यूशन विज़ार्ड द्वारा उपयोग किया जा सकता है या नहीं। |

### setShowIndent(boolean value) {#setShowIndent-boolean-}
```
public final void setShowIndent(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि इस आउटलाइन कोड के इंडेंट दिखाए जाने चाहिए या नहीं।

--------------------

यह MS Project 2010 प्रॉपर्टी के लिए नया है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि इस आउटलाइन कोड के इंडेंट्स दिखाए जाने चाहिए या नहीं। |

