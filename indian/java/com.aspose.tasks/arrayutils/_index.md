---
title: "ArrayUtils"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ArrayList प्रोसेसिंग के लिए उपयोगी क्लास।"
type: docs
weight: 14
url: /hi/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

ArrayList प्रोसेसिंग के लिए उपयोगी क्लास।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | निर्दिष्ट स्थिति से शुरू करके प्रत्येक सूची तत्व पर एल्गोरिदम लागू करें। |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | निर्दिष्ट शर्त के आधार पर ArrayList तत्वों को फ़िल्टर करें। |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | निर्दिष्ट शर्त को पूरा करने वाले ArrayList तत्व की पहली उपस्थिति खोजें। |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| ऐरेज़ | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


निर्दिष्ट स्थिति से शुरू करके प्रत्येक सूची तत्व पर एल्गोरिदम लागू करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| array | java.util.List | प्रसंस्करण के लिए ArrayList। |
| एल्गोरिदम | com.aspose.tasks.IAlgorithm | लागू किया गया एल्गोरिद्म। |
| startIndex | int | प्रारंभिक तत्व की स्थिति। |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


निर्दिष्ट शर्त के आधार पर ArrayList तत्वों को फ़िल्टर करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| array | java.util.List | प्रक्रिया करने के लिए सूची। |
| cond | com.aspose.tasks.ICondition | सूची को फ़िल्टर करने के लिए उपयोग की जाने वाली शर्त। |

**Returns:**
java.util.List - फ़िल्टर की गई सूची।
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


निर्दिष्ट शर्त को पूरा करने वाले ArrayList तत्व की पहली उपस्थिति खोजें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| array | java.util.List | प्रसंस्करण के लिए ArrayList। |
| cond | com.aspose.tasks.ICondition | ArrayList तत्व को खोजने के लिए उपयोग की जाने वाली शर्त। |

**Returns:**
java.lang.Object - सूची तत्व या null।
