---
title: "Aspose::Tasks::Project::GetDuration メソッド"
linktitle: "GetDuration"
articleTitle: "GetDuration"
second_title: "Aspose.Tasks for C++"
description: "プロジェクトの設定 Prj::DurationFormat で定義されたデフォルトの期間形式と、指定された単位数を持つ Duration オブジェクトを取得します。"
type: docs
weight: 1080
url: /ja/cpp/aspose.tasks/project/getduration/
---

## GetDuration (1 of 3) {#getduration_1}

プロジェクトの設定 Prj::DurationFormat で定義されたデフォルトの期間形式と、指定された単位数を持つ Duration オブジェクトを取得します。

**Returns:** Duration object.

```cpp
GetDuration(double val)
```

| パラメーター | 説明 |
| --- | --- |
| 値 | 指定された単位数。 |

---

## GetDuration (2 of 3) {#getduration_2}

指定された数の TimeUnitType 単位を持つ Duration オブジェクトを取得します。

**Returns:** Duration object.

```cpp
GetDuration(double val, TimeUnitType timeUnit)
```

| パラメーター | 説明 |
| --- | --- |
| 値 | 指定された単位数。 |
| timeUnit | 指定された TimeUnitType 値。 |

---

## GetDuration (3 of 3) {#getduration_3}

指定された TimeSpan 値と指定された TimeUnitType 値を持つ Duration オブジェクトを取得します。

**Returns:** Duration object.

```cpp
GetDuration(System::TimeSpan timeSpan, TimeUnitType timeUnit)
```

| パラメーター | 説明 |
| --- | --- |
| timeSpan | 指定された TimeSpan 値。 |
| timeUnit | 指定された TimeUnitType 値。 |

