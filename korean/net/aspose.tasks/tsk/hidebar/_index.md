---
title: "Tsk.HideBar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. Microsoft Project에 표시될 때 작업의 간트 바가 숨겨지는지 여부를 결정합니다."
type: docs
weight: 480
url: /ko/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Microsoft Project에 표시될 때 작업의 간트 바가 숨겨져 있는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## 예제

Tsk.HideBar 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


