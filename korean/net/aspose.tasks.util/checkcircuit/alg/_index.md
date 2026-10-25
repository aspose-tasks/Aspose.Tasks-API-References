---
title: "CheckCircuit.Alg"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CheckCircuit 메서드. 지정된 객체가 이미 처리되었는지 확인합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

지정된 객체가 이미 처리되었는지 확인합니다.

```csharp
public override void Alg(Task el, int level)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | 작업 | 처리할 객체. |
| 레벨 | Int32 | 트리 노드 레벨. |

## 예제

손상된 프로젝트 구조를 감지하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// 프로젝트 구조를 확인합니다.
// 프로젝트 구조가 올바르지 않을 경우 <see cref="TasksException">가 발생합니다.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


