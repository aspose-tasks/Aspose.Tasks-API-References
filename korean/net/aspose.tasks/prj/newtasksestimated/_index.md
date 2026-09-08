---
title: "Prj.NewTasksEstimated"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 기본적으로 추정 기간이 표시되는지 여부를 결정합니다."
type: docs
weight: 570
url: /ko/net/aspose.tasks/prj/newtasksestimated/
---
## Prj.NewTasksEstimated field

예상 기간이 기본적으로 표시되는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEstimated;
```

## 예제

Prj.NewTasksEstimated 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.NewTasksEstimated, true);

Console.WriteLine("New Tasks Estimated: " + project.Get(Prj.NewTasksEstimated));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


