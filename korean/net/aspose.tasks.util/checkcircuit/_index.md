---
title: "클래스 CheckCircuit"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Util.CheckCircuit 클래스. 작업 트리에서 회로가 포함되어 있는지 확인합니다."
type: docs
weight: 2680
url: /ko/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

작업 트리(트리)가 회로를 포함하고 있는지 확인합니다.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | `CheckCircuit` 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | 지정된 객체가 이미 처리되었는지 확인합니다. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


