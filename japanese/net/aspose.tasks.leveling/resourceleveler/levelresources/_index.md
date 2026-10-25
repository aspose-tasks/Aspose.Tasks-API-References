---
title: "ResourceLeveler.LevelResources"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "ResourceLeveler メソッド。指定されたリソースに対して、指定されたレベリングオプションを使用してタスクをレベル付けします。"
type: docs
weight: 30
url: /ja/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

指定されたレベリング オプションを使用して、指定されたリソースのタスクをレベル調整します。

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| プロジェクト | プロジェクト | リソースレベリングを適用するプロジェクト。 |
| オプション | LevelingOptions | リソースをどのようにレベル付けするかを指定するオプション。 |

### 戻り値

リソースレベリングの結果を含むオブジェクト。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | パラメーター options が null の場合。 |

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


