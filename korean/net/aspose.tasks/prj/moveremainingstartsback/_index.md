---
title: "Prj.MoveRemainingStartsBack"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 상태 날짜 이후에 시작하도록 예약되었지만 더 일찍 시작된 작업의 남은 부분 시작 시점을 상태 날짜로 되돌릴지 여부를 결정합니다."
type: docs
weight: 510
url: /ko/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

상태 날짜 이후에 시작하도록 예정되었으나 실제로는 더 일찍 시작된 작업의 남은 부분 시작을 상태 날짜로 되돌릴지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## 예제

Prj.MoveRemainingStartsBack 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


