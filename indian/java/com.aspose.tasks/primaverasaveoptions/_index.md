---
title: "PrimaveraSaveOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Primavera XER फ़ॉर्मेट में प्रोजेक्ट सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 208
url: /hi/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Primavera XER फ़ॉर्मेट में प्रोजेक्ट सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | एक नया उदाहरण प्रारंभ करता है [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले वृद्धि को प्राप्त करता है। |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले उपसर्ग को प्राप्त करता है। |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले प्रत्यय को प्राप्त करता है। |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या गतिविधि IDs को पुनः क्रमांकित करने की आवश्यकता है। |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | एक मान प्राप्त करता है जो दर्शाता है कि निर्यात के दौरान संसाधनों के असाइनमेंट को सारांश टास्क में छोड़ना चाहिए या नहीं। |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले वृद्धि को सेट करता है। |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले उपसर्ग को सेट करता है। |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले प्रत्यय को सेट करता है। |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | एक मान सेट करता है जो यह दर्शाता है कि क्या गतिविधि IDs को पुनः क्रमांकित करने की आवश्यकता है। |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | एक मान सेट करता है जो दर्शाता है कि निर्यात के दौरान संसाधनों के असाइनमेंट को सारांश टास्क में छोड़ना चाहिए या नहीं। |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


एक नया उदाहरण प्रारंभ करता है [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) क्लास का।

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले वृद्धि को प्राप्त करता है।

**Returns:**
int - गतिविधि IDs को पुनः क्रमांकित करने में उपयोग किया जाने वाला वृद्धि मान।
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले उपसर्ग को प्राप्त करता है।

**Returns:**
java.lang.String - गतिविधि IDs को पुनः क्रमांकित करने में उपयोग किया जाने वाला उपसर्ग।
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले प्रत्यय को प्राप्त करता है।

**Returns:**
int - गतिविधि IDs को पुनः क्रमांकित करने में उपयोग किया जाने वाला प्रत्यय।
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या गतिविधि IDs को पुनः क्रमांकित करने की आवश्यकता है।

**Returns:**
boolean - एक मान जो यह दर्शाता है कि क्या गतिविधि IDs को पुनः क्रमांकित करने की आवश्यकता है।
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


एक मान प्राप्त करता है जो दर्शाता है कि निर्यात के दौरान संसाधनों के असाइनमेंट को सारांश टास्क में छोड़ना चाहिए या नहीं।

Primavera सॉफ़्टवेयर संसाधनों को सारांश (WBS) कार्यों को असाइन करने का समर्थन नहीं करता है। इसलिए, ऐसे असाइनमेंट्स का निर्यात Primavera के मॉडल के अनुसार एक अमान्य फ़ाइल का परिणाम दे सकता है। यदि true है, तो निर्यात के दौरान सारांश कार्यों को असाइनमेंट्स को छोड़ दिया जाता है। यदि false (डिफ़ॉल्ट मान) है, तो निर्यात के दौरान सारांश कार्य को असाइनमेंट मिलने पर एक अपवाद फेंका जाएगा।

**Returns:**
boolean - यह दर्शाने वाला मान कि निर्यात के दौरान संसाधनों को सारांश कार्यों को असाइनमेंट्स को छोड़ना चाहिए या नहीं।
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले वृद्धि को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | गतिविधि IDs को पुनः क्रमांकित करने में उपयोग किया जाने वाला वृद्धि मान। |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले उपसर्ग को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | गतिविधि IDs को पुनः क्रमांकित करने में उपयोग किया जाने वाला उपसर्ग। |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


गतिविधि IDs के पुनः क्रमांकन में उपयोग किए जाने वाले प्रत्यय को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | गतिविधि IDs को पुनः क्रमांकित करने में उपयोग किया जाने वाला प्रत्यय। |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि क्या गतिविधि IDs को पुनः क्रमांकित करने की आवश्यकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो यह दर्शाता है कि क्या गतिविधि IDs को पुनः क्रमांकित करने की आवश्यकता है। |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि निर्यात के दौरान संसाधनों के असाइनमेंट को सारांश टास्क में छोड़ना चाहिए या नहीं।

Primavera सॉफ़्टवेयर संसाधनों को सारांश (WBS) कार्यों को असाइन करने का समर्थन नहीं करता है। इसलिए, ऐसे असाइनमेंट्स का निर्यात Primavera के मॉडल के अनुसार एक अमान्य फ़ाइल का परिणाम दे सकता है। यदि true है, तो निर्यात के दौरान सारांश कार्यों को असाइनमेंट्स को छोड़ दिया जाता है। यदि false (डिफ़ॉल्ट मान) है, तो निर्यात के दौरान सारांश कार्य को असाइनमेंट मिलने पर एक अपवाद फेंका जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि निर्यात के दौरान संसाधनों को सारांश कार्यों को असाइनमेंट्स को छोड़ना चाहिए या नहीं। |

