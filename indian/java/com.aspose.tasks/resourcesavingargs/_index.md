---
title: "ResourceSavingArgs"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "यह क्लास बाहरी संसाधन फ़ाइलों को सहेजने से संबंधित डेटा के सेट का प्रतिनिधित्व करती है, जो HTML प्रारूप में रूपांतरण के दौरान होता है।"
type: docs
weight: 254
url: /hi/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

यह क्लास उन डेटा सेट का प्रतिनिधित्व करती है जो बाहरी संसाधन फ़ाइल की सहेजने से संबंधित है, जो HTML प्रारूप में रूपांतरण के दौरान होती है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | यदि KeepStreamOpen गलत है तो स्ट्रीम बंद करें, अन्यथा इसे फ्लश करें। |
| [getFileName()](#getFileName--) | कनवर्टर से कस्टम मेथड के कोड तक जाने वाले अनुमानित फ़ाइल नाम को प्राप्त करता है। |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | संसाधन सहेजने के समाप्त होने के बाद स्ट्रीम को खुला रखने का संकेत देने वाला मान प्राप्त करता है। |
| [getStream()](#getStream--) | सहेजी गई फ़ाइल की बाइनरी सामग्री प्राप्त करता है। |
| [getUri()](#getUri--) | संसाधन URI प्राप्त करता है। |
| [setFileName(String value)](#setFileName-java.lang.String-) | कनवर्टर से कस्टम मेथड के कोड तक जाने वाले अनुमानित फ़ाइल नाम को सेट करता है। |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | संसाधन सहेजने के समाप्त होने के बाद स्ट्रीम को खुला रखने का संकेत देने वाला मान सेट करता है। |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | सहेजी गई फ़ाइल की बाइनरी सामग्री सेट करता है। |
| [setUri(String value)](#setUri-java.lang.String-) | संसाधन URI सेट करता है। |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


यदि KeepStreamOpen गलत है तो स्ट्रीम बंद करें, अन्यथा इसे फ्लश करें।

### getFileName() {#getFileName--}
```
public final String getFileName()
```


कनवर्टर से कस्टम मेथड के कोड तक जाने वाले अनुमानित फ़ाइल नाम को प्राप्त करता है। इसे कस्टम कोड में यह तय करने के लिए उपयोग किया जा सकता है कि फ़ाइल को कैसे प्रोसेस किया जाए या कहां सहेजा जाए।

**Returns:**
java.lang.String - कनवर्टर से कस्टम मेथड के कोड तक जाने वाला अनुमानित फ़ाइल नाम।
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


संसाधन सहेजने के समाप्त होने के बाद स्ट्रीम को खुला रखने का संकेत देने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि संसाधन सहेजने के समाप्त होने के बाद स्ट्रीम खुला रहेगा या नहीं।
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


सहेजी गई फ़ाइल की बाइनरी सामग्री प्राप्त करता है।

**Returns:**
java.io.OutputStream - सहेजी गई फ़ाइल की बाइनरी सामग्री।
### getUri() {#getUri--}
```
public final String getUri()
```


संसाधन URI प्राप्त करता है।

**Returns:**
java.lang.String - संसाधन URI।
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


कनवर्टर से कस्टम मेथड के कोड तक जाने वाले अनुमानित फ़ाइल नाम को सेट करता है। इसे कस्टम कोड में यह तय करने के लिए उपयोग किया जा सकता है कि फ़ाइल को कैसे प्रोसेस किया जाए या कहां सहेजा जाए।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | कनवर्टर से कस्टम मेथड के कोड तक जाने वाला अनुमानित फ़ाइल नाम। |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


संसाधन सहेजने के समाप्त होने के बाद स्ट्रीम को खुला रखने का संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि संसाधन सहेजने के समाप्त होने के बाद स्ट्रीम खुला रहेगा या नहीं। |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


सहेजी गई फ़ाइल की बाइनरी सामग्री सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.io.OutputStream | सहेजी गई फ़ाइल की बाइनरी सामग्री। |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


संसाधन URI सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | संसाधन URI। |

