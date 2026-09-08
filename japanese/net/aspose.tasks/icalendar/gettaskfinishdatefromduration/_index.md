---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "ICalendar method. タスクの開始日を分割した部分と作業期間から、タスクの完了日時を計算します"
type: docs
weight: 50
url: /ja/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

タスクの開始日、分割部分、作業期間からタスクの終了日時を計算します。

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| タスク | タスク | 完了日を計算するタスク。 |
| duration | TimeSpan | 計算する期間。 |

### 戻り値

指定された開始日と期間に対するタスクの完了日。

## 備考

タスクがサマリーであるか、nullであるか、開始日が設定されていない場合は DateTime.MinValue を返します。

### 関連項目

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


