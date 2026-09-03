---
title: "Aspose::Tasks::ResourceAssignment::MakeTPs メソッド"
linktitle: "MakeTPs"
articleTitle: "MakeTPs"
second_title: "Aspose.Tasks for C++"
description: "時間別データのリストを生成します。"
type: docs
weight: 740
url: /ja/cpp/aspose.tasks/resourceassignment/maketps/
---

## MakeTPs {#maketps}

時間別データのリストを生成します。

**Returns:** A maximum date from list or start date if list is empty.

```cpp
MakeTPs(System::DateTime start, System::TimeSpan time, const System::SharedPtr< Calendar > & calendar, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Aspose::Tasks::TimephasedData >>> & list, bool isWorking, int32_t type)
```

| パラメーター | 説明 |
| --- | --- |
| 開始 | 指定された開始日です。 |
| 時間 | 指定された作業時間です。 |
| カレンダー | 指定された作業カレンダーです。 |
| リスト | 時間フェーズデータのリストです。 |
| isWorking | 時間フェーズデータが作業中かどうかを指定するフラグです。 |
| type | 指定された時間フェーズデータ型です。 |

