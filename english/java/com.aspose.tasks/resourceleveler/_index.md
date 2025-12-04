---
title: ResourceLeveler
second_title: Aspose.Tasks for Java API Reference
description: Contains resource leveling methods.
type: docs
weight: 252
url: /java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Contains resource leveling methods.
## Constructors

| Constructor | Description |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Methods

| Method | Description |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Clears any leveling delay that was previously added to the project during resource leveling. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Clears any leveling delay that was previously added to the specified tasks during resource leveling. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Levels tasks for all project's resources using default leveling options. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Levels tasks for the specified resources using the specified leveling options. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Clears any leveling delay that was previously added to the project during resource leveling.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project to clear leveling. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Clears any leveling delay that was previously added to the specified tasks during resource leveling.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tasks | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | The enumerable containing tasks for which leveling delay should be cleared. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Levels tasks for all project's resources using default leveling options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project to apply resource leveling. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Levels tasks for the specified resources using the specified leveling options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project to apply resource leveling. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Options which specifies how to level resources. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
