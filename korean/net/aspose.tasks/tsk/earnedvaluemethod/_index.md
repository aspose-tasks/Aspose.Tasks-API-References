---
title: "Tsk.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 수행된 작업의 예산 비용(BCWP)을 계산하기 위해 Complete 또는 Physical Complete 필드를 사용할지 여부를 결정합니다."
type: docs
weight: 350
url: /ko/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

% 완료 또는 물리적 % 완료 필드를 사용하여 수행된 작업의 예산 비용(BCWP)을 계산할지 여부를 결정합니다.

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## 예제

Tsk.EarnedValueMethod 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


