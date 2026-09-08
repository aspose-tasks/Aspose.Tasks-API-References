---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Aspose.Tasks for .NET API 참조"
description: "FieldHelper 메서드. 특정 작업 필드의 기본 제목을 반환합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

특정 작업 필드의 기본 제목을 반환합니다.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| taskKey | TaskKey | 기본 제목을 가져올 작업 필드. |

### 반환 값

필드가 MS Project 뷰에 표시될 수 있으면 특정 작업 필드의 기본 제목을 반환하고, 그렇지 않으면 null을 반환합니다.

## 예제

특정 작업 필드의 기본 제목을 가져오는 방법을 보여줍니다.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### 또 보기

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


