---
title: "Aspose::Tasks::Project::Recalculate メソッド"
linktitle: "Recalculate"
articleTitle: "Recalculate"
second_title: "Aspose.Tasks for C++"
description: "すべてのプロジェクト タスクの ID、アウトライン レベル、開始/終了日を再スケジュールし、早期/遅延日を設定し、余裕時間、作業およびコスト フィールドを計算します。"
type: docs
weight: 1130
url: /ja/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

すべてのプロジェクト タスクの ID、アウトライン レベル、開始/終了日を再スケジュールし、早期/遅延日を設定し、余裕時間、作業およびコスト フィールドを計算します。

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

すべてのプロジェクトタスクの ID、アウトラインレベル、開始/終了日を再スケジュールし、早期/遅延日を設定し、スラック、作業およびコストフィールドをオプションの検証とともに計算します。

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| パラメーター | 説明 |
| --- | --- |
| 検証 | true の場合、再計算の検証が実行されます。検証対象データ: 現在、タスクおよびタスクリンクの日付範囲に対する基本的な検証のみが実装されています。タスクの日付範囲（例: ActualStart - ActualFinish、EarlyStart - EarlyFinish など）およびタスクリンクの日付は、開始日が終了日以下であるという日付基準に対してチェックされます。上記の条件のいずれかが失敗した場合、RecalculationValidationException がスローされます。 |

