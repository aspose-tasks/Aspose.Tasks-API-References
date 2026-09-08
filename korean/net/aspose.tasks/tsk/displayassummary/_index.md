---
title: "Tsk.DisplayAsSummary"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업을 요약 작업으로 표시할지 여부를 결정합니다. 읽기는 XML 형식만 지원됩니다"
type: docs
weight: 280
url: /ko/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

작업을 요약 작업으로 표시할지 여부를 결정합니다. 읽기는 XML 형식만 지원됩니다.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## 예제

Tsk.DisplayAsSummary 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


