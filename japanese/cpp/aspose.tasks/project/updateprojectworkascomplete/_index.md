---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete メソッド"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks for C++"
description: "プロジェクト全体の指定された日付まで、すべての作業を完了として更新します。"
type: docs
weight: 2080
url: /ja/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

プロジェクト全体の指定された日付まで、すべての作業を完了として更新します。

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| パラメーター | 説明 |
| --- | --- |
| completeThrough | 作業を完了として更新する日付です。 |
| setZeroOrHundredPercentCompleteOnly | true に設定すると、完了までの日付が指定された日付より前のタスクのみを 100% 完了として更新します。false の場合、予定開始日と完了までの日付に基づいて完了率の値を計算します。 |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

指定されたタスクのリストに対して、指定された日付までのすべての作業を完了として更新します。

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| パラメーター | 説明 |
| --- | --- |
| completeThrough | 作業を完了として更新する日付です。 |
| setZeroOrHundredPercentCompleteOnly | true に設定すると、完了までの日付が指定された日付より前のタスクのみを 100% 完了として更新します。false の場合、予定開始日と完了までの日付に基づいて完了率の値を計算します。 |
| taskCollection | 作業を更新するタスクの List< Task >。 |

