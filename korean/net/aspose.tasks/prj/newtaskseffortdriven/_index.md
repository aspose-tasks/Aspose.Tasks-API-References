---
title: "Prj.NewTasksEffortDriven"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 새 작업이 노력 기반인지 여부를 결정합니다"
type: docs
weight: 560
url: /ko/net/aspose.tasks/prj/newtaskseffortdriven/
---
## Prj.NewTasksEffortDriven field

새 작업이 노력 기반인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEffortDriven;
```

## 예제

Prj.NewTasksEffortDriven 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.NewTasksEffortDriven, true);

Console.WriteLine("New Tasks Effort Driven: " + project.Get(Prj.NewTasksEffortDriven));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


