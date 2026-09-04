---
title: "ResourceLeveler"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحتوي على أساليب تسوية الموارد."
type: docs
weight: 253
url: /ar/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

يحتوي على أساليب تسوية الموارد.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | يمسح أي تأخير في التسوية تم إضافته مسبقًا إلى المشروع أثناء تسوية الموارد. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | يمسح أي تأخير في التسوية تم إضافته مسبقًا إلى المهام المحددة أثناء تسوية الموارد. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | يقوم بتسوية المهام لجميع موارد المشروع باستخدام خيارات التسوية الافتراضية. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | يقوم بتسوية المهام للموارد المحددة باستخدام خيارات التسوية المحددة. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


يمسح أي تأخير في التسوية تم إضافته مسبقًا إلى المشروع أثناء تسوية الموارد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | مشروع لمسح التسوية. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


يمسح أي تأخير في التسوية تم إضافته مسبقًا إلى المهام المحددة أثناء تسوية الموارد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المهام | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | المجموعة القابلة للتعداد التي تحتوي على المهام التي يجب مسح تأخير التسوية لها. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


يقوم بتسوية المهام لجميع موارد المشروع باستخدام خيارات التسوية الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | مشروع لتطبيق تسوية الموارد. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


يقوم بتسوية المهام للموارد المحددة باستخدام خيارات التسوية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | مشروع لتطبيق تسوية الموارد. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | الخيارات التي تحدد كيفية تسوية الموارد. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
