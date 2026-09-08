---
title: "Prj.MoveCompletedEndsForward"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 상태 날짜 이전에 완료될 예정이었지만 나중에 시작된 작업의 완료된 부분 끝을 상태 날짜로 앞당길지 여부를 결정합니다"
type: docs
weight: 500
url: /ko/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

상태 날짜 이전에 완료될 예정이었지만 나중에 시작된 작업의 완료된 부분 끝을 상태 날짜로 앞당길지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## 예제

Prj.MoveCompletedEndsForward 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


