---
title: "クラス LevelingResult"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.Leveling.LevelingResult クラス。リソースレベリングの結果を表します。"
type: docs
weight: 960
url: /ja/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

リソースレベリングの結果を表します。

```csharp
public sealed class LevelingResult
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [LevelingResult](levelingresult/)() | `LevelingResult` クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | リソースレベリングの影響を受けたタスクの集合を取得します。 |

## 例

デフォルトオプションを使用してプロジェクトのすべてのリソースをレベル設定する方法を示します。

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### 関連項目

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


