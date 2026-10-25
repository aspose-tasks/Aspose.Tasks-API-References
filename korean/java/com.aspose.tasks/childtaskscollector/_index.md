---
title: "ChildTasksCollector"
second_title: "Aspose.Tasks for Java API Reference"
description: "모든 하위 작업을 수집합니다."
type: docs
weight: 49
url: /ko/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

모든 하위 작업을 수집합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | 새로운 [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | 지정된 객체를 처리합니다. |
| [getTasks()](#getTasks--) | 수집된 하위 객체(작업) 목록을 가져옵니다. |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


새로운 [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) 클래스 인스턴스를 초기화합니다.

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


지정된 객체를 처리합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | 처리할 객체. |
| 레벨 | int | 트리 노드 레벨. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


수집된 하위 객체(작업) 목록을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - 수집된 하위 객체(작업) 목록.
