---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "ResourceAssignment メソッド。指定された日時間隔の時間別作業量を取得します。"
type: docs
weight: 730
url: /ja/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

指定された日時間隔の時間別作業量を取得します。

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| start | DateTime | 日時間隔の開始。 |
| 終了 | DateTime | 日時間隔の終了。 |
| timephasedDataType | TimephasedDataType | 使用する時間別データのタイプ。 |

## 例

任意の日時間隔に対する割り当て作業の計算方法を示します。

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// 各時間ごとの assignmen の作業を出力します。
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### 関連項目

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

指定された日時間隔の時間別作業量を取得します。

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| start | DateTime | 日時間隔の開始。 |
| 終了 | DateTime | 日時間隔の終了。 |

### 関連項目

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


