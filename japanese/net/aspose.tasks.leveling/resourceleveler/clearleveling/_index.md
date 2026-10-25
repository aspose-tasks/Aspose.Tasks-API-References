---
title: "ResourceLeveler.ClearLeveling"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "ResourceLeveler メソッド。リソースレベリング中にプロジェクトに以前追加されたレベリング遅延をすべてクリアします。"
type: docs
weight: 10
url: /ja/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

リソース レベリング中にプロジェクトに以前追加されたレベリング遅延をすべてクリアします。

```csharp
public static void ClearLeveling(Project project)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| プロジェクト | プロジェクト | レベリングをクリアするプロジェクト。 |

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

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

リソース レベリング中に指定されたタスクに以前追加されたレベリング遅延をすべてクリアします。

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| タスク | IEnumerable`1 | レベル遅延をクリアすべきタスクを含む列挙体です。 |

### 関連項目

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


