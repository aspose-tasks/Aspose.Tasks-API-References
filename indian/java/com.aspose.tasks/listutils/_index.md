---
title: "ListUtils"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "सूची प्रसंस्करण के लिए उपयोगिता क्लास।"
type: docs
weight: 147
url: /hi/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

सूची प्रसंस्करण के लिए उपयोगिता क्लास।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | निर्दिष्ट स्थिति से शुरू होकर प्रत्येक सूची तत्व पर एल्गोरिदम लागू करें। |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | निर्दिष्ट शर्त के अनुसार सूची तत्वों को फ़िल्टर करें। |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | निर्दिष्ट शर्त को पूरा करने वाले सूची तत्व की पहली उपस्थिति खोजें। |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


निर्दिष्ट स्थिति से शुरू होकर प्रत्येक सूची तत्व पर एल्गोरिदम लागू करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूची | java.util.List&lt;T&gt; | प्रक्रिया करने के लिए सूची। |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | लागू किया गया एल्गोरिद्म। |
| startIndex | int | प्रारंभिक तत्व की स्थिति। |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


निर्दिष्ट शर्त के अनुसार सूची तत्वों को फ़िल्टर करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूची | java.util.List&lt;T&gt; | प्रक्रिया करने के लिए एक सूची। |
| cond | [ICondition](../../com.aspose.tasks/icondition) | निर्दिष्ट सूची को फ़िल्टर करने के लिए प्रयुक्त शर्त। |

**Returns:**
java.util.List&lt;T&gt; - फ़िल्टर की गई सूची।
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


निर्दिष्ट शर्त को पूरा करने वाले सूची तत्व की पहली उपस्थिति खोजें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूची | java.util.List&lt;T&gt; | प्रक्रिया करने के लिए एक सूची। |
| cond | [ICondition](../../com.aspose.tasks/icondition) | निर्दिष्ट सूची में तत्व खोजने के लिए प्रयुक्त शर्त। |
| clazz | java.lang.Class | तत्व T का क्लास प्रकार। |

**Returns:**
T - सूची तत्व या null।
