---
title: "Prj.DurationFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 전체 기간을 표현하는 형식"
type: docs
weight: 300
url: /ko/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

대량 기간을 표현하는 형식.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## 예제

Prj.DurationFormat 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


