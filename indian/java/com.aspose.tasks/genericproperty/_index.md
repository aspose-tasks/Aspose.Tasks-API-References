---
title: "GenericProperty"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "कंटेनर प्रॉपर्टी का प्रतिनिधित्व करता है।"
type: docs
weight: 113
url: /hi/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

कंटेनर प्रॉपर्टी का प्रतिनिधित्व करता है।

TKey : प्रॉपर्टी मान का प्रकार।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | एक नया उदाहरण प्रारंभ करता है GenericProperty&lt;T&gt; क्लास का। |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | एक नया उदाहरण प्रारंभ करता है GenericProperty&lt;TKey&gt; स्ट्रक्ट का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | एक मान लौटाता है जो दर्शाता है कि निर्दिष्ट `obj1` उदाहरण `obj2` उदाहरण के बराबर है या नहीं। |
| [Clone()](#Clone--) | इस उदाहरण की एक डीप कॉपी बनाता और लौटाता है। |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | उदाहरण की एक डीप कॉपी बनाकर उसे दूसरे उदाहरण में रखता है। |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | प्रॉपर्टी का नाम प्राप्त करता है। |
| [getValue()](#getValue--) | प्रॉपर्टी का मान प्राप्त करता है। |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


एक नया उदाहरण प्रारंभ करता है GenericProperty&lt;T&gt; क्लास का।

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


एक नया उदाहरण प्रारंभ करता है GenericProperty&lt;TKey&gt; स्ट्रक्ट का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | प्रॉपर्टी का नाम। |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


एक मान लौटाता है जो दर्शाता है कि निर्दिष्ट `obj1` उदाहरण `obj2` उदाहरण के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | तुलना करने के लिए पहला ऑब्जेक्ट। |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | तुलना करने के लिए दूसरा ऑब्जेक्ट। |

**Returns:**
boolean - यदि निर्दिष्ट `obj1` उदाहरण निर्दिष्ट `obj2` उदाहरण के बराबर है तो true लौटाता है; अन्यथा false।
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


इस उदाहरण की एक डीप कॉपी बनाता और लौटाता है।

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


उदाहरण की एक डीप कॉपी बनाकर उसे दूसरे उदाहरण में रखता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | एक अन्य उदाहरण। |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
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
### getName() {#getName--}
```
public final String getName()
```


प्रॉपर्टी का नाम प्राप्त करता है।

**Returns:**
java.lang.String - प्रॉपर्टी का नाम।
### getValue() {#getValue--}
```
public final Object getValue()
```


प्रॉपर्टी का मान प्राप्त करता है।

**Returns:**
java.lang.Object - प्रॉपर्टी का मान।
