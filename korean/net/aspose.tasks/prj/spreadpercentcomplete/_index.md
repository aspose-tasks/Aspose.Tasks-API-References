---
title: "Prj.SpreadPercentComplete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 완료 비율이 상태 날짜에 퍼지는지 여부를 결정합니다"
type: docs
weight: 670
url: /ko/net/aspose.tasks/prj/spreadpercentcomplete/
---
## Prj.SpreadPercentComplete field

완료 비율이 상태 날짜까지 분배되는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadPercentComplete;
```

## 예제

Prj.SpreadPercentComplete 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.SpreadPercentComplete, true);

Console.WriteLine("Spread Percent Complete: " + project.Get(Prj.SpreadPercentComplete));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


