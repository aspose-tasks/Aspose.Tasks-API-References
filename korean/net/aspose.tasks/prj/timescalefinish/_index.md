---
title: "Prj.TimescaleFinish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 보기에서 시간 눈금이 종료되는 날짜입니다."
type: docs
weight: 730
url: /ko/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

보기에서 시간 눈금이 끝나는 날짜.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## 예제

Prj.TimescaleFinish 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


