---
title: "ChildTasksCollector"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "सभी चाइल्ड टास्क एकत्र करता है।"
type: docs
weight: 49
url: /hi/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

सभी चाइल्ड टास्क एकत्र करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | नए [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) वर्ग का एक नया उदाहरण आरंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | निर्दिष्ट ऑब्जेक्ट को प्रोसेस करता है। |
| [getTasks()](#getTasks--) | संकलित चाइल्ड ऑब्जेक्ट्स (कार्य) की सूची प्राप्त करता है। |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


नए [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) वर्ग का एक नया उदाहरण आरंभ करता है।

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


निर्दिष्ट ऑब्जेक्ट को प्रोसेस करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | प्रोसेस करने के लिए वस्तु। |
| स्तर | int | ट्री नोड स्तर। |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


संकलित चाइल्ड ऑब्जेक्ट्स (कार्य) की सूची प्राप्त करता है।

**Returns:**
java.util.List<com.aspose.tasks.Task> - संकलित चाइल्ड ऑब्जेक्ट्स (कार्य) की सूची।
