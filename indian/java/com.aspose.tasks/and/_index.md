---
title: "और"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "निर्दिष्ट शर्तों पर लॉजिकल AND लागू करता है।"
type: docs
weight: 10
url: /hi/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

निर्दिष्ट शर्तों पर लॉजिकल AND लागू करता है।

T : मेथड इंटरफ़ेस लागू करने के लिए ऑब्जेक्ट का प्रकार।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | And&lt;T&gt; क्लास का नया उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [check(T el)](#check-T-) | यदि निर्दिष्ट वस्तु शर्तों को पूरा करती है तो true लौटाता है। |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


And&lt;T&gt; क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | पहली शर्त। |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | दूसरी शर्त। |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


यदि निर्दिष्ट वस्तु शर्तों को पूरा करती है तो true लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | जाँचने के लिए ऑब्जेक्ट। |

**Returns:**
boolean - यदि वस्तु शर्तों को पूरा करती है तो True।
