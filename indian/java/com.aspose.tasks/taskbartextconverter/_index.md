---
title: "TaskBarTextConverter"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "टास्क डेटा को बार टेक्स्ट में बदलने वाला कस्टम कन्वर्टर।"
type: docs
weight: 290
url: /hi/java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

कार्य के डेटा को बार टेक्स्ट में बदलने के लिए कस्टम कनवर्टर।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | कार्य के डेटा को बार टेक्स्ट में बदलने के लिए कस्टम कनवर्टर। |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


कार्य के डेटा को बार टेक्स्ट में बदलने के लिए कस्टम कनवर्टर।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | टास्क जिसके लिए टास्क बार का टेक्स्ट रेंडर किया जाएगा। |

**Returns:**
java.lang.String - निर्दिष्ट टास्क के अनुरूप बार के लिए रेंडर करने वाला टेक्स्ट।
