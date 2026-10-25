---
title: "RemoveTask"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "निर्दिष्ट कार्य को कार्यों के पेड़ से हटाता है।"
type: docs
weight: 246
url: /hi/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

निर्दिष्ट कार्य को कार्यों के पेड़ से हटाता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | नया उदाहरण प्रारंभ करता है [RemoveTask](../../com.aspose.tasks/removetask) वर्ग का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | कुछ न करें। |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | कुछ न करें। |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | निर्दिष्ट मूल कार्य से कार्य को हटाता है। |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


नया उदाहरण प्रारंभ करता है [RemoveTask](../../com.aspose.tasks/removetask) वर्ग का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | हटाने के लिए कार्य। |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


कुछ न करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | प्रोसेस करने के लिए वस्तु। |
| स्तर | int | ट्री नोड स्तर। |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


कुछ न करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | प्रोसेस करने के लिए वस्तु। |
| स्तर | int | ट्री नोड स्तर। |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


निर्दिष्ट मूल कार्य से कार्य को हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | मूल कार्य। |
| स्तर | int | ट्री नोड स्तर। |

