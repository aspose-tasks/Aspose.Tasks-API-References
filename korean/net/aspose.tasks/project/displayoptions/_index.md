---
title: "Project.DisplayOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. ProjectDisplayOptions 클래스의 인스턴스를 가져옵니다"
type: docs
weight: 380
url: /ko/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

[`ProjectDisplayOptions`](../../projectdisplayoptions/) 클래스의 인스턴스를 가져옵니다.

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## 예제

프로젝트의 표시 옵션을 조정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Project가 수동으로 예약된 작업과 가능한 일정 충돌을 식별할 때 경고를 표시할지 여부를 나타내는 값을 설정합니다.
// 이 옵션은 Project 2010 버전 이상에서 사용할 수 있습니다.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### 또 보기

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


