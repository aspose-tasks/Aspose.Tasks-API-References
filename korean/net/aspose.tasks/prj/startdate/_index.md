---
title: "Prj.StartDate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트의 시작 날짜"
type: docs
weight: 680
url: /ko/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

프로젝트 시작 날짜.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## 예제

Prj.StartDate 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


