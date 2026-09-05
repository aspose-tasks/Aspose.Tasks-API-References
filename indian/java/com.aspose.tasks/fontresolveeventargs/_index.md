---
title: "FontResolveEventArgs"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "फ़ॉन्ट समाधान होने पर कॉल किए जाने वाले कॉलबैक के लिए तर्क प्रदान करता है।"
type: docs
weight: 99
url: /hi/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

फ़ॉन्ट समाधान होने पर कॉल किए जाने वाले कॉलबैक के लिए तर्क प्रदान करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | अनुरोधित फ़ॉन्ट का नाम प्राप्त करता है। |
| [getResolvedFontName()](#getResolvedFontName--) | सुलझाए गए फ़ॉन्ट का नाम प्राप्त करता है। |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | सुलझाए गए फ़ॉन्ट का नाम सेट करता है। |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


अनुरोधित फ़ॉन्ट का नाम प्राप्त करता है।

**Returns:**
java.lang.String - अनुरोधित फ़ॉन्ट का नाम।
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


सुलझाए गए फ़ॉन्ट का नाम प्राप्त करता है। दृश्य को रेंडर करने के लिए उपयोग किए जाने वाले फ़ॉन्ट को नियंत्रित करने के लिए इसे सेट किया जा सकता है।

**Returns:**
java.lang.String - यदि फ़ॉन्ट मिला तो अनुरोधित फ़ॉन्ट का नाम, या फॉलबैक फ़ॉन्ट का नाम, या यदि फ़ॉन्ट नहीं मिला तो null।
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


सुलझाए गए फ़ॉन्ट का नाम सेट करता है। दृश्य को रेंडर करने के लिए उपयोग किए जाने वाले फ़ॉन्ट को नियंत्रित करने के लिए इसे सेट किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | सुलझाए गए फ़ॉन्ट का नाम। |

