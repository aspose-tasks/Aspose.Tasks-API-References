---
title: "Calendar.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Calendar プロパティ。Primavera 形式から読み込まれたカレンダーの Primavera 固有プロパティを含むオブジェクトを取得します"
type: docs
weight: 100
url: /ja/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Primavera 形式から読み込まれたカレンダーの Primavera 固有プロパティを含むオブジェクトを取得します。

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## 例

Primavera ファイルからプロジェクトを読み取り、カレンダーの Primavera 固有プロパティを調べる方法を示します。

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// 特別な Uid を持つプロジェクトを返します。
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### 関連項目

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


