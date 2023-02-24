---
title: RescheduleUncompletedWorkToStartAfter
second_title: Aspose.Tasks for .NET API リファレンス
description: 未完了のプロジェクト作業を指定された日付以降に開始するように再スケジュールします
type: docs
weight: 1170
url: /ja/net/aspose.tasks/project/rescheduleuncompletedworktostartafter/
---
## RescheduleUncompletedWorkToStartAfter(DateTime) {#rescheduleuncompletedworktostartafter}

未完了のプロジェクト作業を、指定された日付以降に開始するように再スケジュールします。

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| after | DateTime | 未完了の作業を再スケジュールする日付。 |

### 備考

このメソッドを使用する前に、Project.CanSplitsInProgressTasks フラグが true に設定されていることを確認してください。

### 関連項目

* class [Project](../)
* 名前空間 [Aspose.Tasks](../../project/)
* 組み立て [Aspose.Tasks](../../../)

---

## RescheduleUncompletedWorkToStartAfter(DateTime, List&lt;Task&gt;) {#rescheduleuncompletedworktostartafter_1}

指定されたタスクのリストの未完了の作業を、指定された日付の後に開始するように再スケジュールします。

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after, List<Task> taskCollection)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| after | DateTime | 未完了の作業を再スケジュールする日付。 |
| taskCollection | List`1 | 未完了の作業を再スケジュールするタスクの List&lt;Task&gt;。 |

### 備考

このメソッドを使用する前に、Project.CanSplitsInProgressTasks フラグが true に設定されていることを確認してください。

### 関連項目

* class [Task](../../task/)
* class [Project](../)
* 名前空間 [Aspose.Tasks](../../project/)
* 組み立て [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->