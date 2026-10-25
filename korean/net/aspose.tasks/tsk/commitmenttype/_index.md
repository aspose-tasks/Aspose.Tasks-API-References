---
title: "Tsk.CommitmentType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 연관된 전달이 있는지 또는 연관된 전달에 대한 종속성이 있는지를 결정합니다. 읽기는 XML 형식만 지원됩니다."
type: docs
weight: 190
url: /ko/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

작업에 연관된 전달이 있는지 또는 연관된 전달에 대한 종속성이 있는지를 결정합니다. 읽기는 XML 형식만 지원됩니다.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## 예제

Tsk.CommitmentType 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


