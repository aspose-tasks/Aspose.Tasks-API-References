---
title: "Prj.SplitsInProgressTasks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 진행 중인 작업을 분할할 수 있는지 여부를 결정합니다"
type: docs
weight: 650
url: /ko/net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

진행 중인 작업을 분할할 수 있는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## 예제

Prj.SplitsInProgressTasks 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


