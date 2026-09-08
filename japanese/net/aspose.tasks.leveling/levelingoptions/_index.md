---
title: "クラス LevelingOptions"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.Leveling.LevelingOptions クラス。リソースレベリングのパラメータを指定できます。"
type: docs
weight: 940
url: /ja/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

リソースレベリングのパラメータを指定できます。

```csharp
public sealed class LevelingOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | `LevelingOptions` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | プロジェクトのレベリング操作をキャンセルするために使用できるトークンを取得または設定します。 |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | レベリング期間の終了日を取得または設定します。デフォルト値はプロジェクト`s 完了日です。 |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | リソース過剰割り当てがあるタスクをレベリングアルゴリズムが遅延させる順序を取得します。過剰割り当てを引き起こすタスクと遅延可能なタスクを特定した後、どのタスクを最初に遅延させるかを指定された順序で使用します。 |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | リソースレベリング中に Aspose.Tasks が生成するログメッセージをインターセプトするために使用できるメッセージハンドラコールバックを取得または設定します。 |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | リソースレベリング中に Aspose.Tasks が出力するログメッセージのレベルを取得または設定します。 |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | レベル設定されるリソースの一覧を取得または設定します。null が設定された場合、プロジェクトのすべてのリソースがレベル設定されます。 |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | レベリング期間の開始日を取得または設定します。デフォルト値はプロジェクト`s 開始日です。 |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


