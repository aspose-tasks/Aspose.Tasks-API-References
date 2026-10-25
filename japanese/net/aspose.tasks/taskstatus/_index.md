---
title: "列挙体 TaskStatus"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.TaskStatus 列挙体。タスクのステータスを指定します。"
type: docs
weight: 2460
url: /ja/net/aspose.tasks/taskstatus/
---
## TaskStatus enumeration

タスクのステータスを指定します。

```csharp
public enum TaskStatus
```

### 値

| 名前 | 値 | 説明 |
| --- | --- | --- |
| Undefined | `-1` | 未定義のタスクステータスです。 |
| Complete | `0` | タスクは 100% 完了しています。 |
| OnSchedule | `1` | ステータス日より前日の少なくともまでに timephased cumulative percent complete が分散されている場合、タスクはスケジュール通りです。 |
| Late | `2` | ステータス日の前日の深夜までに timephased cumulative percent complete が達しない場合、タスクは遅れています。 |
| Future | `3` | タスクの開始日がステータス日より大きい場合、'Future' タスクステータスが設定されます。 |

### 関連項目

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


