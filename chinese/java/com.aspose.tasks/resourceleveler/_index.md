---
title: "ResourceLeveler"
second_title: "Aspose.Tasks for Java API 参考"
description: "包含资源平衡方法。"
type: docs
weight: 253
url: /zh/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

包含资源平衡方法。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | 清除在资源平衡期间先前添加到项目的任何平衡延迟。 |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | 清除在资源平衡期间先前添加到指定任务的任何平衡延迟。 |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | 使用默认平衡选项对项目所有资源的任务进行平衡。 |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | 使用指定的平衡选项对指定资源的任务进行平衡。 |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


清除在资源平衡期间先前添加到项目的任何平衡延迟。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 用于清除平衡的项目。 |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


清除在资源平衡期间先前添加到指定任务的任何平衡延迟。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 任务 | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | 包含应清除平衡延迟的任务的可枚举集合。 |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


使用默认平衡选项对项目所有资源的任务进行平衡。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 用于应用资源平衡的项目。 |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


使用指定的平衡选项对指定资源的任务进行平衡。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 用于应用资源平衡的项目。 |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | 指定资源平衡方式的选项。 |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
