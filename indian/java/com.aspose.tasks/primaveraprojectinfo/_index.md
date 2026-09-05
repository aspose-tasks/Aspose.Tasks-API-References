---
title: "PrimaveraProjectInfo"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Primavera फ़ॉर्मेट से लोड किए गए प्रोजेक्ट के बारे में संक्षिप्त जानकारी दर्शाता है।"
type: docs
weight: 204
url: /hi/java/com.aspose.tasks/primaveraprojectinfo/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectInfo
```

Primavera फ़ॉर्मेट से लोड किए गए प्रोजेक्ट के बारे में संक्षिप्त जानकारी दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getExportFlag()](#getExportFlag--) | प्रोजेक्ट का निर्यात फ़्लैग प्राप्त करता है। |
| [getName()](#getName--) | प्रोजेक्ट का नाम प्राप्त करता है। |
| [getShortName()](#getShortName--) | प्रोजेक्ट का संक्षिप्त नाम (Project ID) प्राप्त करता है। |
| [getUid()](#getUid--) | प्रोजेक्ट का UID प्राप्त करता है। |
### getExportFlag() {#getExportFlag--}
```
public final boolean getExportFlag()
```


प्रोजेक्ट का निर्यात फ़्लैग प्राप्त करता है। जब Primavera में किसी प्रोजेक्ट को निर्यात के लिए चुना जाता है, तो उसका ExportFlag true होता है। कुछ प्रोजेक्ट जो स्पष्ट रूप से निर्यात के लिए नहीं चुने गए हैं, उनके निर्यातित प्रोजेक्ट के संबंध के कारण XER फ़ाइल में निर्यात हो सकते हैं।

**Returns:**
boolean - प्रोजेक्ट का निर्यात फ़्लैग।
### getName() {#getName--}
```
public final String getName()
```


प्रोजेक्ट का नाम प्राप्त करता है।

**Returns:**
java.lang.String - प्रोजेक्ट का नाम।
### getShortName() {#getShortName--}
```
public final String getShortName()
```


प्रोजेक्ट का संक्षिप्त नाम (Project ID) प्राप्त करता है।

**Returns:**
java.lang.String - प्रोजेक्ट का संक्षिप्त नाम (Project ID).
### getUid() {#getUid--}
```
public final int getUid()
```


प्रोजेक्ट का UID प्राप्त करता है।

**Returns:**
int - प्रोजेक्ट का UID।
