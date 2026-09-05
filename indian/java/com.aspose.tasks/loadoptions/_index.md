---
title: "LoadOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "फ़ाइल या स्ट्रीम से प्रोजेक्ट लोड करते समय अतिरिक्त लोड पैरामीटर निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 148
url: /hi/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

फ़ाइल या स्ट्रीम से प्रोजेक्ट लोड करते समय अतिरिक्त लोड पैरामीटर निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | एक नया उदाहरण प्रारंभ करता है [LoadOptions](../../com.aspose.tasks/loadoptions) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | एक टोकन प्राप्त करता है जिसका उपयोग प्रोजेक्ट लोडिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है। |
| [getEncoding()](#getEncoding--) | एक एन्कोडिंग प्राप्त करता है जिसका उपयोग HTML, MPX, XER और Primavera XML फ़ॉर्मेट्स से प्रोजेक्ट पढ़ने के लिए किया जाता है। |
| [getErrorHandler()](#getErrorHandler--) | XML पार्स त्रुटियों को संभालने के लिए एक कॉलबैक मेथड प्राप्त करता है। |
| [getPassword()](#getPassword--) | एक प्रोटेक्शन पासवर्ड प्राप्त करता है। |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | एक निर्दिष्ट उदाहरण प्राप्त करता है [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास का, जिसका उपयोग Primavera फ़ॉर्मेट्स (Primavera P6 XER या Primavera P6 Xml) को लोड करने के व्यवहार को अनुकूलित करने के लिए किया जा सकता है। |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | एक टोकन सेट करता है जिसका उपयोग प्रोजेक्ट लोडिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है। |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | एन्कोडिंग सेट करता है जिसका उपयोग HTML, MPX, XER और Primavera XML फ़ॉर्मेट्स से प्रोजेक्ट पढ़ने के लिए किया जाता है। |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | XML पार्स त्रुटियों को संभालने के लिए एक कॉलबैक मेथड सेट करता है। |
| [setPassword(String value)](#setPassword-java.lang.String-) | एक प्रोटेक्शन पासवर्ड सेट करता है। |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | एक निर्दिष्ट उदाहरण सेट करता है [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास का, जिसका उपयोग Primavera फ़ॉर्मेट्स (Primavera P6 XER या Primavera P6 Xml) को लोड करने के व्यवहार को अनुकूलित करने के लिए किया जा सकता है। |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


एक नया उदाहरण प्रारंभ करता है [LoadOptions](../../com.aspose.tasks/loadoptions) क्लास का।

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


एक टोकन प्राप्त करता है जिसका उपयोग प्रोजेक्ट लोडिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है।

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


एक एन्कोडिंग प्राप्त करता है जिसका उपयोग HTML, MPX, XER और Primavera XML फ़ॉर्मेट्स से प्रोजेक्ट पढ़ने के लिए किया जाता है। डिफ़ॉल्ट एन्कोडिंग UTF8 है।

**Returns:**
java.nio.charset.Charset - एन्कोडिंग जिसका उपयोग HTML, MPX, XER और Primavera XML फ़ॉर्मेट्स से प्रोजेक्ट पढ़ने के लिए किया जाता है।
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


XML पार्स त्रुटियों को संभालने के लिए एक कॉलबैक मेथड प्राप्त करता है।

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


एक प्रोटेक्शन पासवर्ड प्राप्त करता है।

**Returns:**
java.lang.String - एक प्रोटेक्शन पासवर्ड।
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


एक निर्दिष्ट उदाहरण प्राप्त करता है [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास का, जिसका उपयोग Primavera फ़ॉर्मेट्स (Primavera P6 XER या Primavera P6 Xml) को लोड करने के व्यवहार को अनुकूलित करने के लिए किया जा सकता है।

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


एक टोकन सेट करता है जिसका उपयोग प्रोजेक्ट लोडिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | एक टोकन जिसका उपयोग प्रोजेक्ट लोडिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है। |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


एन्कोडिंग सेट करता है जिसका उपयोग HTML, MPX, XER और Primavera XML फ़ॉर्मेट्स से प्रोजेक्ट पढ़ने के लिए किया जाता है। डिफ़ॉल्ट एन्कोडिंग UTF8 है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.nio.charset.Charset | एन्कोडिंग जिसका उपयोग HTML, MPX, XER और Primavera XML फ़ॉर्मेट्स से प्रोजेक्ट पढ़ने के लिए किया जाता है। |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


XML पार्स त्रुटियों को संभालने के लिए एक कॉलबैक मेथड सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML पार्स त्रुटियों को संभालने के लिए एक कॉलबैक मेथड। |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


एक प्रोटेक्शन पासवर्ड सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | एक सुरक्षा पासवर्ड। |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


एक निर्दिष्ट उदाहरण सेट करता है [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास का, जिसका उपयोग Primavera फ़ॉर्मेट्स (Primavera P6 XER या Primavera P6 Xml) को लोड करने के व्यवहार को अनुकूलित करने के लिए किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | Primavera फ़ॉर्मेट्स (Primavera P6 XER या Primavera P6 Xml) को लोड करने के व्यवहार को अनुकूलित करने के लिए उपयोग किया जा सकने वाला [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) क्लास का निर्दिष्ट इंस्टेंस। |

