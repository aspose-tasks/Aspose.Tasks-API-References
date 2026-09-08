---
title: "LevelingOptions.MessageLevel"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "LevelingOptions プロパティ。リソース レベリング中に Aspose.Tasks が出力するログ メッセージのレベルを取得または設定します"
type: docs
weight: 60
url: /ja/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

リソースレベリング中に Aspose.Tasks が出力するログメッセージのレベルを取得または設定します。

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


