---
title: "Prj.TimescaleStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 보기에서 시간 눈금이 시작되는 날짜입니다."
type: docs
weight: 740
url: /ko/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

보기에서 시간 눈금이 시작되는 날짜.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## 예제

보기가 시작되어야 하는 날짜를 조정하기 위해 시간 눈금 시작 날짜를 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


