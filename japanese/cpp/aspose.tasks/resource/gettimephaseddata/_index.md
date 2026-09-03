---
title: "Aspose::Tasks::Resource::GetTimephasedData メソッド"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks for C++"
description: "指定された開始日と終了日の範囲内の TimephasedData 値を含む、このオブジェクトの TimephasedDataCollection を返します。"
type: docs
weight: 850
url: /ja/cpp/aspose.tasks/resource/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

指定された開始日と終了日の範囲内の TimephasedData 値を含む、このオブジェクトの TimephasedDataCollection を返します。

**Returns:** List of Aspose::Tasks::TimephasedData .

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| パラメーター | 説明 |
| --- | --- |
| 開始 | 時間フェーズデータの開始日です。 |
| end | 時間分割データの終了日です。 |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

このオブジェクトの TimephasedDataCollection クラスのインスタンスを返します。指定された TimephasedDataType の開始日と終了日の範囲内にある TimephasedData の値が含まれます。

**Returns:** List of TimephasedData .

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| パラメーター | 説明 |
| --- | --- |
| 開始 | 時間フェーズデータの開始日です。 |
| end | 時間分割データの終了日です。 |
| timephasedType | 時間分割データのタイプ ( Aspose::Tasks::TimephasedDataType )です。 |

