---
title: "Tsk.IsActive"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 활성 상태인지 여부를 결정합니다. 비활성 작업은 더 이상 다른 작업이나 전체 프로젝트 일정에 영향을 주지 않습니다."
type: docs
weight: 550
url: /ko/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

작업이 활성 상태인지 여부를 결정합니다. 비활성 작업은 더 이상 다른 작업이나 전체 프로젝트 일정에 영향을 주지 않습니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## 예제

Tsk.IsActive 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


