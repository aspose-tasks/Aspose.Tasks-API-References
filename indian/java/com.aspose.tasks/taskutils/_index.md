---
title: "TaskUtils"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "टास्क के साथ उपयोगी ऑपरेशन्स प्रदान करने वाली हेल्पर क्लास।"
type: docs
weight: 307
url: /hi/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

टास्क के साथ उपयोगी ऑपरेशन्स प्रदान करने वाली हेल्पर क्लास।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | निर्दिष्ट एल्गोरिद्म को ट्री के प्रत्येक कार्य पर लागू करता है। |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | शर्त को पूरा करने वाले कार्यों का नया ट्री बनाता है। |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | कार्य ट्री में शर्त को पूरा करने वाला कार्य खोजता है। |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | सभी स्तरों पर पुनरावर्ती रूप से कार्य के चाइल्ड कार्यों की संख्या की गणना करता है। |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


निर्दिष्ट एल्गोरिद्म को ट्री के प्रत्येक कार्य पर लागू करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | ट्री की जड़ |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | लागू किया गया एल्गोरिद्म। |
| स्तर | int | जड़ कार्य का स्तर। |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


शर्त को पूरा करने वाले कार्यों का नया ट्री बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | ट्री की जड़। |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | लागू की गई शर्त। |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


कार्य ट्री में शर्त को पूरा करने वाला कार्य खोजता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | ट्री की जड़। |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | लागू की गई शर्त। |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


सभी स्तरों पर पुनरावर्ती रूप से कार्य के चाइल्ड कार्यों की संख्या की गणना करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | वह कार्य जिसके बच्चों की गणना की जाती है। |

**Returns:**
int - बच्चों की संख्या।
