---
title: "Aspose::Tasks::ICalendar::GetWorkingHours method"
linktitle: "GetWorkingHours"
articleTitle: "GetWorkingHours"
second_title: "Aspose.Tasks for C++"
description: "指定された日付の作業時間数を返します。"
type: docs
weight: 60
url: /ja/cpp/aspose.tasks/icalendar/getworkinghours/
---

## GetWorkingHours (1 of 2) {#getworkinghours_1}

指定された日付の作業時間数を返します。

**Returns:** Working hours at the specified date.

```cpp
GetWorkingHours(System::DateTime dt)
```

| パラメーター | 説明 |
| --- | --- |
| dt | 作業時間を取得する対象の日付。 |

---

## GetWorkingHours (2 of 2) {#getworkinghours_2}

指定された日時間隔の作業時間の WorkUnit（開始、終了、期間）を返します。

**Returns:** Instance of WorkUnit class containing Start, Finish and Duration of working hours.

```cpp
GetWorkingHours(System::DateTime start, System::DateTime finish)
```

| パラメーター | 説明 |
| --- | --- |
| 開始 | 間隔の開始日です。 |
| 終了 | 間隔の終了日です。 |

