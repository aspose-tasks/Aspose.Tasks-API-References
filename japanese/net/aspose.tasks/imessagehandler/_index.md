---
title: "インターフェイス IMessageHandler"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.IMessageHandler インターフェイス。リソースレベリングの結果を受け取るコールバックを表します。"
type: docs
weight: 880
url: /ja/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

リソースレベリングの結果を受け取るコールバックを表します。

```csharp
public interface IMessageHandler
```

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks はメッセージを出力するときにこのメソッドを呼び出します。 |

## 例

特定のリソースをレベル調整する方法、レベル調整オプションをカスタマイズする方法、そしてレベル調整アルゴリズムのメッセージを確認する方法を示します。

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

### 関連項目

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


