---
title: "कुंजी"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "निर्दिष्ट प्रकार की क्लास की प्रॉपर्टी कुंजी को दर्शाता है।"
type: docs
weight: 139
url: /hi/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

निर्दिष्ट प्रकार की क्लास की एक प्रॉपर्टी कुंजी को दर्शाता है। इस क्लास का एक इंस्टेंस कंटेनर की प्रॉपर्टी प्राप्त करने या सेट करने के समय उपयोग किया जाता है।

T : प्रॉपर्टी मान का प्रकार।
K : प्रॉपर्टी कुंजी का प्रकार।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [Clone()](#Clone--) | इंस्टेंस की गहरी कॉपी लौटाता है। |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | उदाहरण की एक डीप कॉपी बनाकर उसे दूसरे उदाहरण में रखता है। |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | एक मान लौटाता है जो दर्शाता है कि निर्दिष्ट `obj1` उदाहरण `obj2` उदाहरण के बराबर है या नहीं। |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | प्रॉपर्टी की कुंजी प्राप्त करता है। |
| [hashCode()](#hashCode--) | Key क्लास के इंस्टेंस के लिए हैश कोड लौटाता है। |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


इंस्टेंस की गहरी कॉपी लौटाता है।

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


उदाहरण की एक डीप कॉपी बनाकर उसे दूसरे उदाहरण में रखता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | एक अन्य उदाहरण। |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### equals(Key obj1, Key obj2) {#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-}
```
public static boolean equals(Key obj1, Key obj2)
```


एक मान लौटाता है जो दर्शाता है कि निर्दिष्ट `obj1` उदाहरण `obj2` उदाहरण के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | तुलना करने के लिए पहला ऑब्जेक्ट। |
| obj2 | com.aspose.tasks.Key | तुलना करने के लिए दूसरा ऑब्जेक्ट। |

**Returns:**
boolean - यदि निर्दिष्ट `obj1` उदाहरण निर्दिष्ट `obj2` उदाहरण के बराबर है तो true लौटाता है; अन्यथा false।
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


प्रॉपर्टी की कुंजी प्राप्त करता है।

**Returns:**
K - प्रॉपर्टी की कुंजी।
### hashCode() {#hashCode--}
```
public int hashCode()
```


Key क्लास के इंस्टेंस के लिए हैश कोड लौटाता है।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड लौटाता है।
