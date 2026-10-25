---
title: "Rsc.AvailableTo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 현재 기간에 지정된 단위로 리소스가 작업에 사용할 수 있는 종료 날짜"
type: docs
weight: 130
url: /ko/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

리소스가 현재 기간에 지정된 단위로 작업 가능해지는 종료 날짜.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## 예제

Rsc.AvailableTo 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


