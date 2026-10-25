---
title: "ResourceLeveler"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "संसाधन स्तरन विधियों को शामिल करता है।"
type: docs
weight: 253
url: /hi/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

संसाधन स्तरन विधियों को शामिल करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | संसाधन स्तरन के दौरान प्रोजेक्ट में पहले जोड़ा गया कोई भी स्तरन विलंब साफ़ करता है। |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | निर्दिष्ट कार्यों के लिए संसाधन लेवलिंग के दौरान पहले जो लेवलिंग देरी जोड़ी गई थी, उसे साफ़ करता है। |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | डिफ़ॉल्ट लेवलिंग विकल्पों का उपयोग करके सभी प्रोजेक्ट के संसाधनों के लिए कार्यों को लेवल करता है। |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | निर्दिष्ट लेवलिंग विकल्पों का उपयोग करके निर्दिष्ट संसाधनों के लिए कार्यों को लेवल करता है। |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


संसाधन स्तरन के दौरान प्रोजेक्ट में पहले जोड़ा गया कोई भी स्तरन विलंब साफ़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | लेवलिंग को साफ़ करने के लिए प्रोजेक्ट। |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


निर्दिष्ट कार्यों के लिए संसाधन लेवलिंग के दौरान पहले जो लेवलिंग देरी जोड़ी गई थी, उसे साफ़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कार्य | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | लेवलिंग देरी को साफ़ करने वाले कार्यों को शामिल करने वाला एन्यूमेरेबल। |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


डिफ़ॉल्ट लेवलिंग विकल्पों का उपयोग करके सभी प्रोजेक्ट के संसाधनों के लिए कार्यों को लेवल करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | संसाधन लेवलिंग लागू करने के लिए प्रोजेक्ट। |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


निर्दिष्ट लेवलिंग विकल्पों का उपयोग करके निर्दिष्ट संसाधनों के लिए कार्यों को लेवल करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | संसाधन लेवलिंग लागू करने के लिए प्रोजेक्ट। |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | विकल्प जो निर्धारित करता है कि संसाधनों को कैसे लेवल किया जाए। |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
