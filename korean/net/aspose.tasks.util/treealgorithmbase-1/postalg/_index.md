---
title: "TreeAlgorithmBase1.PostAlg"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TreeAlgorithmBase 메서드. 트리 노드 처리 후에 호출됩니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.util/treealgorithmbase-1/postalg/
---
## TreeAlgorithmBase&lt;T&gt;.PostAlg method

트리 노드 처리 후에 호출됩니다.

```csharp
public virtual void PostAlg(T el, int level)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리할 노드. |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


