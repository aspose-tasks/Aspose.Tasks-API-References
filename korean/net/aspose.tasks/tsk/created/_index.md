---
title: "Tsk.Created"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 생성된 날짜"
type: docs
weight: 250
url: /ko/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

작업이 생성된 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## 예제

Tsk.Created 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


