---
title: "Prj.BaselineForEarnedValue"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj field. 분산 값을 계산하는 데 사용되는 특정 기준선"
type: docs
weight: 80
url: /ko/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

분산 값을 계산하는 데 사용되는 특정 기준선.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## 예제

Prj.BaselineForEarnedValue 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


