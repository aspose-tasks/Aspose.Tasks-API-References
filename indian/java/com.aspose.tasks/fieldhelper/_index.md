---
title: "FieldHelper"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "फ़ील्ड्स के साथ उपयोगी संचालन प्रदान करने वाली सहायक क्लास।"
type: docs
weight: 88
url: /hi/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

फ़ील्ड्स के साथ उपयोगी संचालन प्रदान करने वाली सहायक क्लास।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | विशिष्ट फ़ील्ड का डिफ़ॉल्ट शीर्षक लौटाता है। |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | निर्दिष्ट कार्य फ़ील्ड का डिफ़ॉल्ट शीर्षक लौटाता है। |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


विशिष्ट फ़ील्ड का डिफ़ॉल्ट शीर्षक लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ील्ड | int | डिफ़ॉल्ट शीर्षक प्राप्त करने के लिए फ़ील्ड। |

**Returns:**
java.lang.String - यदि फ़ील्ड को MS Project के दृश्य में दिखाया जा सकता है तो निर्दिष्ट फ़ील्ड का डिफ़ॉल्ट शीर्षक, अन्यथा null।
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


निर्दिष्ट कार्य फ़ील्ड का डिफ़ॉल्ट शीर्षक लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| taskKey | byte | डिफ़ॉल्ट शीर्षक प्राप्त करने के लिए कार्य फ़ील्ड। |

**Returns:**
java.lang.String - यदि फ़ील्ड को MS Project के दृश्य में दिखाया जा सकता है तो निर्दिष्ट कार्य फ़ील्ड का डिफ़ॉल्ट शीर्षक, अन्यथा null।
