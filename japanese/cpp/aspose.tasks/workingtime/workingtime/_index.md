---
title: "Aspose::Tasks::WorkingTime::WorkingTime コンストラクタ"
linktitle: "WorkingTime"
articleTitle: "WorkingTime"
second_title: "Aspose.Tasks for C++"
description: "指定された開始時刻と終了時刻を持つ間隔で WorkingTime クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/workingtime/workingtime/
---

## WorkingTime (1 of 3) {#workingtime_1}

指定された開始時刻と終了時刻を持つ間隔で WorkingTime クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::DateTime fromTime, System::DateTime toTime)
```

| パラメーター | 説明 |
| --- | --- |
| fromTime | 間隔の開始時刻 |
| toTime | 間隔の終了時刻 |

---

## WorkingTime (2 of 3) {#workingtime_2}

指定された開始時刻と終了時刻を持つ間隔項目で WorkingTime クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::TimeSpan fromTime, System::TimeSpan toTime)
```

| パラメーター | 説明 |
| --- | --- |
| fromTime | 間隔の開始時刻は TimeSpan 構造体で表されます。 |
| toTime | 間隔の終了時刻は TimeSpan 構造体で表されます。 |

---

## WorkingTime (3 of 3) {#workingtime_3}

指定された開始時刻と終了時刻を持つ間隔項目で WorkingTime クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(int32_t fromHours, int32_t toHours)
```

| パラメーター | 説明 |
| --- | --- |
| fromHours | 間隔の開始時刻は 0〜24 の整数時間で表されます。 |
| toHours | 間隔の終了時刻は 0〜24 の整数時間で表されます。 |

