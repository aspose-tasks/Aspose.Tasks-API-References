---
title: "Prj.MoveRemainingStartsForward"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 나중에 시작하도록 예정된 작업의 남은 부분 시작이 상태 날짜로 앞당겨야 하는지 여부를 결정합니다"
type: docs
weight: 520
url: /ko/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

나중에 시작하도록 예정된 작업의 남은 부분 시작을 상태 날짜로 앞당길지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## 예제

Prj.MoveRemainingStartsForward 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


