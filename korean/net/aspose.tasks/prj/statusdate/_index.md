---
title: "Prj.StatusDate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 진행 상황을 표시하거나 획득 가치 총계를 계산하기 위한 상태 날짜. 별도의 상태 날짜가 지정되지 않는 한 상태 날짜는 현재 날짜(오늘 날짜)와 동일합니다."
type: docs
weight: 690
url: /ko/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

진행 상황을 표시하거나 획득 가치 총계를 계산하기 위한 상태 날짜입니다. 별도의 상태 날짜가 지정되지 않는 한 상태 날짜는 현재 날짜(오늘 날짜)와 동일합니다.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## 예제

Prj.StatusDate 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


