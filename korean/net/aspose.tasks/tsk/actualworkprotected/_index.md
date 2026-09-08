---
title: "Tsk.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 실제 작업이 보호되는 기간. 읽기는 XML 형식에서만 지원됩니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

실제 작업이 보호되는 기간. 읽기는 XML 형식만 지원됩니다.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## 예제

Tsk.ActualWorkProtected 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


