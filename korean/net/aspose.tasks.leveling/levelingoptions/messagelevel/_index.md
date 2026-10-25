---
title: "LevelingOptions.MessageLevel"
second_title: "Aspose.Tasks for .NET API 참조"
description: "LevelingOptions 속성. 리소스 레벨링 중 Aspose.Tasks에서 발생하는 로그 메시지 수준을 가져오거나 설정합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

리소스 레벨링 중 Aspose.Tasks에서 발생하는 로그 메시지 수준을 가져오거나 설정합니다.

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


