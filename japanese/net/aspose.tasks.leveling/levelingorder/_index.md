---
title: "Enum LevelingOrder"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.Leveling.LevelingOrder enum. レベリング順序の可能な値を定義します"
type: docs
weight: 950
url: /ja/net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

レベリング順序の可能な値を定義します。

```csharp
public enum LevelingOrder
```

### 値

| 名前 | 値 | 説明 |
| --- | --- | --- |
| Standard | `1` | 考慮されるプロパティは次のとおりです: 前任タスクの関係、総余裕時間（総余裕時間が大きいタスクが最初に遅延されます）、開始日、優先度。これはデフォルト値です。 |
| IdOnly | `2` | タスクは ID の昇順で遅延されます。 |
| PriorityThenStandard | `3` | 優先度が最初に考慮され、次に Standard と同じプロパティが適用されます。 |

### 関連項目

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


