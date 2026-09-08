---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 프로젝트 리소스 할당 목록에서 잘못된 리소스 할당을 제거합니다."
type: docs
weight: 1170
url: /ko/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

프로젝트 리소스 할당 목록에서 잘못된 리소스 할당을 제거합니다.

```csharp
public void RemoveInvalidResourceAssignments()
```

## 비고

MS Project는 각 작업에 대해 빈 리소스 할당을 생성합니다. 해당 메서드를 호출하여 이를 제거합니다.

## 예제

잘못된 할당을 제거하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// 잘못된 할당 제거
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


