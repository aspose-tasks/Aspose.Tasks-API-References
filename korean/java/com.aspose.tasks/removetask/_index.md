---
title: "RemoveTask"
second_title: "Aspose.Tasks for Java API Reference"
description: "지정된 작업을 작업 트리에서 제거합니다."
type: docs
weight: 246
url: /ko/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

지정된 작업을 작업 트리에서 제거합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | [RemoveTask](../../com.aspose.tasks/removetask) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | 아무 것도 하지 않습니다. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | 아무 것도 하지 않습니다. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | 지정된 상위 작업에서 작업을 제거합니다. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


[RemoveTask](../../com.aspose.tasks/removetask) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 제거할 작업. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


아무 것도 하지 않습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 처리할 객체. |
| 레벨 | int | 트리 노드 레벨. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


아무 것도 하지 않습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 처리할 객체. |
| 레벨 | int | 트리 노드 레벨. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


지정된 상위 작업에서 작업을 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 상위 작업. |
| 레벨 | int | 트리 노드 레벨. |

