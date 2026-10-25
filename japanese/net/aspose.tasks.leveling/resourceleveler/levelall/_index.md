---
title: "ResourceLeveler.LevelAll"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "ResourceLeveler メソッド。デフォルトのレベル設定オプションを使用して、すべてのプロジェクトリソースのタスクをレベル調整します。"
type: docs
weight: 20
url: /ja/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

デフォルトのレベリング オプションを使用して、プロジェクトのすべてのリソースのタスクをレベル調整します。

```csharp
public static LevelingResult LevelAll(Project project)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| プロジェクト | プロジェクト | リソースレベリングを適用するプロジェクト。 |

### 戻り値

リソースレベリングの結果を含むオブジェクト。

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


