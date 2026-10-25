---
title: "Not"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "निर्दिष्ट शर्त पर लॉजिकल NOT लागू करता है।"
type: docs
weight: 162
url: /hi/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

निर्दिष्ट शर्त पर लॉजिकल NOT लागू करता है।

T : मेथड इंटरफ़ेस लागू करने के लिए ऑब्जेक्ट का प्रकार।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | एक नई Not&lt;T&gt; क्लास का उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [check(T el)](#check-T-) | यदि निर्दिष्ट ऑब्जेक्ट शर्त को पूरा करता है तो true लौटाता है। |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


एक नई Not&lt;T&gt; क्लास का उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | निर्दिष्ट शर्त। |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


यदि निर्दिष्ट ऑब्जेक्ट शर्त को पूरा करता है तो true लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | जाँचने के लिए ऑब्जेक्ट। |

**Returns:**
boolean - यदि ऑब्जेक्ट शर्त को पूरा करता है तो True।
