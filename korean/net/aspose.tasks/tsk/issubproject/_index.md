---
title: "Tsk.IsSubproject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 삽입된 프로젝트인지 여부를 결정합니다"
type: docs
weight: 700
url: /ko/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

작업이 삽입된 프로젝트인지 여부를 결정합니다.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## 예제

Tsk.IsSubproject 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


