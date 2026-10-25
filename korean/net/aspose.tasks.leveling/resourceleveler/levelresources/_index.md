---
title: "ResourceLeveler.LevelResources"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceLeveler 메서드. 지정된 레벨링 옵션을 사용하여 지정된 리소스에 대한 작업을 레벨링합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

지정된 레벨링 옵션을 사용하여 지정된 리소스의 작업을 레벨링합니다.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 프로젝트 | Project | 리소스 레벨링을 적용할 프로젝트. |
| 옵션 | LevelingOptions | 리소스를 레벨링하는 방법을 지정하는 옵션. |

### 반환 값

리소스 레벨링 결과를 포함하는 객체.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | 매개변수 options가 null인 경우. |

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


