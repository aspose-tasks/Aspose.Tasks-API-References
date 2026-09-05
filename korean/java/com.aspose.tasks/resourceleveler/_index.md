---
title: "ResourceLeveler"
second_title: "Aspose.Tasks for Java API Reference"
description: "리소스 레벨링 방법을 포함합니다."
type: docs
weight: 253
url: /ko/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

리소스 레벨링 방법을 포함합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | 리소스 레벨링 중에 프로젝트에 이전에 추가된 모든 레벨링 지연을 제거합니다. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | 리소스 레벨링 중에 지정된 작업에 이전에 추가된 모든 레벨링 지연을 제거합니다. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | 기본 레벨링 옵션을 사용하여 프로젝트의 모든 리소스에 대한 작업을 레벨링합니다. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | 지정된 레벨링 옵션을 사용하여 지정된 리소스에 대한 작업을 레벨링합니다. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


리소스 레벨링 중에 프로젝트에 이전에 추가된 모든 레벨링 지연을 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 레벨링을 정리할 프로젝트. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


리소스 레벨링 중에 지정된 작업에 이전에 추가된 모든 레벨링 지연을 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 작업 | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | 레벨링 지연을 제거해야 하는 작업을 포함하는 열거형입니다. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


기본 레벨링 옵션을 사용하여 프로젝트의 모든 리소스에 대한 작업을 레벨링합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 리소스 레벨링을 적용할 프로젝트. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


지정된 레벨링 옵션을 사용하여 지정된 리소스에 대한 작업을 레벨링합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 리소스 레벨링을 적용할 프로젝트. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | 리소스를 레벨링하는 방법을 지정하는 옵션입니다. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
