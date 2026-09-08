---
title: "Tsk.StatusManager"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 현재 작업에 대한 상태 업데이트를 리소스로부터 받는 기업 리소스의 이름"
type: docs
weight: 1050
url: /ko/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

현재 작업에 대한 상태 업데이트를 리소스로부터 받을 기업 리소스의 이름.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## 예제

Tsk.StatusManager 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


