---
title: "Aspose::Tasks::ResourceAssignment::GetTimephasedData メソッド"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks for C++"
description: "TimephasedDataType::AssignmentWork の指定された開始日と終了日の範囲内にある TimephasedData クラスのインスタンスを含む TimephasedDataCollection オブジェクトを返します。"
type: docs
weight: 720
url: /ja/cpp/aspose.tasks/resourceassignment/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

TimephasedDataType::AssignmentWork の指定された開始日と終了日の範囲内にある TimephasedData クラスのインスタンスを含む TimephasedDataCollection オブジェクトを返します。

**Returns:** returns a list containing instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| パラメーター | 説明 |
| --- | --- |
| 開始 | 時間フェーズデータの開始日です。 |
| end | 時間分割データの終了日です。 |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

指定された TimephasedDataType の開始日と終了日の範囲内にある TimephasedData クラスのインスタンスを含む TimephasedDataCollection クラスのインスタンスを返します。

**Returns:** returns a list which contains instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| パラメーター | 説明 |
| --- | --- |
| 開始 | 時間フェーズデータの開始日です。 |
| end | 時間分割データの終了日です。 |
| timephasedType | 時間分割データのタイプ ( Aspose::Tasks::TimephasedDataType )です。 |

