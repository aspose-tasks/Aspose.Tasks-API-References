---
title: "PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Primavera xml फ़ॉर्मेट में प्रोजेक्ट सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 212
url: /hi/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Primavera xml फ़ॉर्मेट में प्रोजेक्ट सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | एक नया उदाहरण प्रारंभ करता है [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | एक मान प्राप्त करता है जो दर्शाता है कि रूट टास्क को सहेजना है या नहीं। |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | एक मान प्राप्त करता है जो दर्शाता है कि निर्यात के दौरान संसाधनों के असाइनमेंट को सारांश टास्क में छोड़ना चाहिए या नहीं। |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | एक मान सेट करता है जो दर्शाता है कि रूट टास्क को सहेजना है या नहीं। |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | एक मान सेट करता है जो दर्शाता है कि निर्यात के दौरान संसाधनों के असाइनमेंट को सारांश टास्क में छोड़ना चाहिए या नहीं। |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


एक नया उदाहरण प्रारंभ करता है [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) क्लास का।

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


एक मान प्राप्त करता है जो दर्शाता है कि रूट टास्क को सहेजना है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि रूट टास्क को सहेजा जाए या नहीं।
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


एक मान प्राप्त करता है जो दर्शाता है कि निर्यात के दौरान संसाधनों के असाइनमेंट को सारांश टास्क में छोड़ना चाहिए या नहीं।

Primavera सॉफ़्टवेयर संसाधनों को सारांश (WBS) कार्यों को असाइन करने का समर्थन नहीं करता है। इसलिए, ऐसे असाइनमेंट्स का निर्यात Primavera के मॉडल के अनुसार एक अमान्य फ़ाइल का परिणाम दे सकता है। यदि true है, तो निर्यात के दौरान सारांश कार्यों को असाइनमेंट्स को छोड़ दिया जाता है। यदि false (डिफ़ॉल्ट मान) है, तो निर्यात के दौरान सारांश कार्य को असाइनमेंट मिलने पर एक अपवाद फेंका जाएगा।

**Returns:**
boolean - यह दर्शाने वाला मान कि निर्यात के दौरान संसाधनों को सारांश कार्यों को असाइनमेंट्स को छोड़ना चाहिए या नहीं।
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि रूट टास्क को सहेजना है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि रूट टास्क को सहेजा जाए या नहीं। |

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

