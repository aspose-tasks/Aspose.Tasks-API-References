---
title: "Tsk.IsSubprojectReadOnly"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 하위 프로젝트가 읽기 전용인지 여부를 결정합니다"
type: docs
weight: 710
url: /ko/net/aspose.tasks/tsk/issubprojectreadonly/
---
## Tsk.IsSubprojectReadOnly field

하위 프로젝트가 읽기 전용인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsSubprojectReadOnly;
```

## 예제

Tsk.IsSubprojectReadOnly 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubprojectReadOnly, true);

Console.WriteLine("Is Subproject Read Only: " + task.Get(Tsk.IsSubprojectReadOnly));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


