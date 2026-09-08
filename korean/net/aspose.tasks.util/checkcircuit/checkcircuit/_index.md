---
title: "CheckCircuit.CheckCircuit"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CheckCircuit 생성자. CheckCircuit 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

[`CheckCircuit`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public CheckCircuit()
```

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

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


