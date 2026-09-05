---
title: "TaskUtils"
second_title: "Aspose.Tasks for Java API Reference"
description: "작업에 대한 유용한 연산을 제공하는 도우미 클래스."
type: docs
weight: 307
url: /ko/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

작업에 대한 유용한 연산을 제공하는 도우미 클래스.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | 지정된 알고리즘을 트리의 각 작업에 적용합니다. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | 조건을 만족하는 작업들의 새 트리를 구축합니다. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | 작업 트리에서 조건을 만족하는 작업을 찾습니다. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | 재귀적으로 모든 레벨을 통해 작업의 하위 작업 수를 계산합니다. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


지정된 알고리즘을 트리의 각 작업에 적용합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | 트리의 루트 |
| 알고리즘 | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | 적용된 알고리즘. |
| 레벨 | int | 루트 작업의 레벨. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


조건을 만족하는 작업들의 새 트리를 구축합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | 트리의 루트. |
| 조건 | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | 적용된 조건. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


작업 트리에서 조건을 만족하는 작업을 찾습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | 트리의 루트. |
| 조건 | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | 적용된 조건. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


재귀적으로 모든 레벨을 통해 작업의 하위 작업 수를 계산합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 자식 작업을 계산하는 작업. |

**Returns:**
int - 자식 수.
