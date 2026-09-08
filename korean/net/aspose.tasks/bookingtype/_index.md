---
title: "열거형 BookingType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.BookingType 열거형. 리소스의 예약 유형을 지정합니다."
type: docs
weight: 150
url: /ko/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

리소스의 예약 유형을 지정합니다.

```csharp
public enum BookingType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 원본 프로젝트 파일에 값이 정의되지 않았음을 나타냅니다. |
| Committed | `0` | Committed 예약 유형을 나타냅니다. |
| Proposed | `1` | Proposed 예약 유형을 나타냅니다. |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

Asn.BookingType 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


