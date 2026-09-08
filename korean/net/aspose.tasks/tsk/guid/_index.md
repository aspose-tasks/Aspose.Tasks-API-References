---
title: "Tsk.Guid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 대해 생성된 고유 식별 코드입니다."
type: docs
weight: 460
url: /ko/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

작업에 대해 생성된 고유 식별 코드.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## 예제

Tsk.Guid 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


