---
title: "클래스 LevelingOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Leveling.LevelingOptions 클래스. 리소스 레벨링 매개변수를 지정할 수 있습니다."
type: docs
weight: 940
url: /ko/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

리소스 레벨링 매개변수를 지정할 수 있습니다.

```csharp
public sealed class LevelingOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | `LevelingOptions` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | 프로젝트 레벨링 작업을 취소하는 데 사용할 수 있는 토큰을 가져오거나 설정합니다. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | 레벨링 기간 종료 날짜를 가져오거나 설정합니다. 기본값은 프로젝트의 종료 날짜입니다. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | 레벨링 알고리즘이 과다 할당된 작업을 지연시키는 순서를 가져옵니다. 과다 할당을 일으키는 작업과 지연될 수 있는 작업을 결정한 후, 지정된 순서에 따라 먼저 지연시킬 작업이 선택됩니다. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | 리소스 레벨링 중 Aspose.Tasks에서 생성된 로그 메시지를 가로챌 수 있는 메시지 핸들러 콜백을 가져오거나 설정합니다. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | 리소스 레벨링 중 Aspose.Tasks에서 발생하는 로그 메시지 수준을 가져오거나 설정합니다. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | 레벨링될 리소스 목록을 가져오거나 설정합니다. null로 설정하면 모든 프로젝트 리소스가 레벨링됩니다. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | 레벨링 기간 시작 날짜를 가져오거나 설정합니다. 기본값은 프로젝트의 시작 날짜입니다. |

## 예제

특정 리소스를 레벨링하는 방법, 레벨링 옵션을 사용자 정의하고 레벨링 알고리즘 메시지를 검사하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### 또 보기

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


