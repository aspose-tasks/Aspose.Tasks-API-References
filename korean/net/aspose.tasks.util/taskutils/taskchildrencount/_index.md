---
title: "TaskUtils.TaskChildrenCount"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskUtils 메서드. 모든 레벨에서 작업 자식 작업 수를 재귀적으로 계산합니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

재귀적으로 모든 레벨에서 작업의 하위 작업 수를 계산합니다.

```csharp
public static int TaskChildrenCount(Task task)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 작업 | 작업 | 자식을 계산하는 작업. |

### 반환 값

자식 수.

## 예제

&lt;see cref=\"Aspose.Tasks.Util.TaskUtils.TaskChildrenCount\" /&gt; 메서드 사용 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 모든 레벨에서 작업의 자식 작업 수를 재귀적으로 계산합니다
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


