---
title: "Tsk.IsPublished"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 현재 작업을 프로젝트의 나머지와 함께 Project Server에 게시할지 여부를 결정합니다."
type: docs
weight: 660
url: /ko/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

현재 작업을 프로젝트의 나머지와 함께 Project Server에 게시해야 하는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## 예제

Tsk.IsPublished 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


