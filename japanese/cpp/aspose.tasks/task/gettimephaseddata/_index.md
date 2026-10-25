---
title: "Aspose::Tasks::Task::GetTimephasedData メソッド"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks for C++"
description: "指定された開始日と終了日の範囲内の TimephasedData 値を含む TimephasedDataCollection オブジェクトを返します。"
type: docs
weight: 1360
url: /ja/cpp/aspose.tasks/task/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

指定された開始日と終了日の範囲内の TimephasedData 値を含む TimephasedDataCollection オブジェクトを返します。

**Returns:** List of Aspose::Tasks::TimephasedData to be filled in.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| パラメーター | 説明 |
| --- | --- |
| 開始 | 時間フェーズデータの開始日です。 |
| end | 時間分割データの終了日です。 |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

指定された時間フェーズデータ型の開始日と終了日の範囲内の TimephasedData 値を含む TimephasedDataCollection オブジェクトを返します。

**Returns:** A TimephasedDataCollection object with TimephasedData values within given start and end dates of specified timephased data type.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| パラメーター | 説明 |
| --- | --- |
| 開始 | 時間フェーズデータの開始日です。 |
| end | 時間分割データの終了日です。 |
| timephasedType | 時間分割データのタイプ ( Aspose::Tasks::TimephasedDataType )です。 |

