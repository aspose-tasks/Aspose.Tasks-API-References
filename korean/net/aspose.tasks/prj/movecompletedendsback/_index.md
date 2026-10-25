---
title: "Prj.MoveCompletedEndsBack"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 상태 날짜 이후에 시작하도록 예정되었지만 더 일찍 시작된 작업의 완료된 부분 끝을 상태 날짜로 되돌릴지 여부를 결정합니다"
type: docs
weight: 490
url: /ko/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

상태 날짜 이후에 시작하도록 예정되었지만 더 일찍 시작된 작업의 완료된 부분 끝을 상태 날짜로 되돌릴지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## 예제

Prj.MoveCompletedEndsBack 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


