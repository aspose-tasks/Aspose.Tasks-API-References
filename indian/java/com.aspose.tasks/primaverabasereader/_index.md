---
title: "PrimaveraBaseReader"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक बेस रीडर का प्रतिनिधित्व करता है जिसका उपयोग मल्टी प्रोजेक्ट Primavera XER या XML फ़ाइलों से प्रोजेक्ट UID पढ़ने के लिए किया जा सकता है।"
type: docs
weight: 196
url: /hi/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

एक बेस रीडर का प्रतिनिधित्व करता है जिसका उपयोग मल्टी प्रोजेक्ट Primavera XER या XML फ़ाइलों से प्रोजेक्ट UID पढ़ने के लिए किया जा सकता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | प्रोजेक्ट की संक्षिप्त जानकारी ऑब्जेक्ट्स की सूची लौटाता है। |
| [getProjectUids()](#getProjectUids--) | प्रोजेक्ट्स के अद्वितीय पहचानकर्ताओं की सूची लौटाता है। |
| [loadProject(int projectUid)](#loadProject-int-) | निर्दिष्ट अद्वितीय पहचानकर्ता के साथ प्रोजेक्ट लोड करता है। |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


प्रोजेक्ट की संक्षिप्त जानकारी ऑब्जेक्ट्स की सूची लौटाता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - प्रोजेक्ट की संक्षिप्त जानकारी ऑब्जेक्ट्स की सूची
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


प्रोजेक्ट्स के अद्वितीय पहचानकर्ताओं की सूची लौटाता है।

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - प्रोजेक्ट्स के अद्वितीय पहचानकर्ताओं की सूची।
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


निर्दिष्ट अद्वितीय पहचानकर्ता के साथ प्रोजेक्ट लोड करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectUid | int | लोड करने के लिए प्रोजेक्ट का अद्वितीय पहचानकर्ता। |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
