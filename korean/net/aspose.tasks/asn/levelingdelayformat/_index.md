---
title: "LevelingDelayFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "지연의 기간 형식."
type: docs
weight: 320
url: /ko/net/aspose.tasks/asn/levelingdelayformat/
---
## Asn.LevelingDelayFormat field

지연의 기간 형식.

```csharp
public static readonly Key<TimeUnitType, AsnKey> LevelingDelayFormat;
```

### 예제

Asn.Delay, Asn.LevelingDelay 및 Asn.LevelingDelayFormat 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Delay, project.GetDuration(0, TimeUnitType.Day));

Console.WriteLine("Delay: " + assignment.Get(Asn.Delay));
Console.WriteLine("Leveling Delay: " + assignment.Get(Asn.LevelingDelay));
Console.WriteLine("Leveling Delay Format: " + assignment.Get(Asn.LevelingDelayFormat));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [TimeUnitType](../../timeunittype)
* enum [AsnKey](../../asnkey)
* class [Asn](../../asn)
* namespace [Aspose.Tasks](../../asn)
* assembly [Aspose.Tasks](../../../)

<!-- 편집 금지: xmldocmd에 의해 Aspose.Tasks.dll용으로 생성됨 -->
