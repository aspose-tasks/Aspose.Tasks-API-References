---
title: CreateCostTimephased
second_title: Aspose.Tasks for .NET API リファレンス
description: の新しいインスタンスを作成して初期化しますTimephasedDataaspose.tasks/timephaseddata/コストベースの時系列データのクラス.
type: docs
weight: 20
url: /ja/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## TimephasedData.CreateCostTimephased method

の新しいインスタンスを作成して初期化します[`TimephasedData`](../)コストベースの時系列データのクラス.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| uid | Int32 | タスクの UID。 |
| start | DateTime | 日時を開始します。 |
| finish | DateTime | 日時を終了します。 |
| value | Double | コスト値。 |
| timeUnit | TimeUnitType | 時間単位のタイプ。 |
| type | TimephasedDataType | 時系列データ型。 |

### 戻り値

のインスタンス[`TimephasedData`](../)コストベースの時系列データのクラス。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | 負のコスト値が指定された場合。 |

### 関連項目

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* 名前空間 [Aspose.Tasks](../../timephaseddata/)
* 組み立て [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->