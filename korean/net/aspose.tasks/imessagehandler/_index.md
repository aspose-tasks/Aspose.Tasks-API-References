---
title: "인터페이스 IMessageHandler"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.IMessageHandler 인터페이스. 리소스 레벨링 결과에 대한 콜백을 나타냅니다"
type: docs
weight: 880
url: /ko/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

리소스 레벨링 결과를 반환하는 콜백을 나타냅니다.

```csharp
public interface IMessageHandler
```

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks는 메시지를 출력할 때 이 메서드를 호출합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


