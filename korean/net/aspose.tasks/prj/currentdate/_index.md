---
title: "Prj.CurrentDate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 시스템 날짜"
type: docs
weight: 190
url: /ko/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

시스템 날짜.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## 예제

Prj.CurrentDate 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


