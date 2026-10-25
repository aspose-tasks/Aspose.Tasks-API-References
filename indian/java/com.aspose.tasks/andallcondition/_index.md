---
title: "AndAllCondition"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "सभी शर्तों पर लॉजिकल AND लागू करता है।"
type: docs
weight: 11
url: /hi/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

सभी शर्तों पर लॉजिकल AND लागू करता है। उदाहरण के लिए: cond1 AND cond2 AND cond3...

T : मेथड इंटरफ़ेस लागू करने के लिए ऑब्जेक्ट का प्रकार।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | AndAllCondition&lt;T&gt; वर्ग का नया उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [check(T el)](#check-T-) | यदि निर्दिष्ट वस्तु शर्तों को पूरा करती है तो true लौटाता है। |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


AndAllCondition&lt;T&gt; वर्ग का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| शर्तें | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | शर्तों की सूची। |

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
