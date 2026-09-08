---
title: "Prj.NewTasksAreManual"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 새 작업이 수동으로 생성되는지 여부를 결정합니다"
type: docs
weight: 550
url: /ko/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

새 작업이 수동으로 생성되는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## 예제

Shows how to read/write Prj.NewTasksAreManual property.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


