---
title: "Prj.DateFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트 보기 날짜 형식"
type: docs
weight: 210
url: /ko/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

프로젝트 보기 날짜 형식.

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## 예제

Prj.DateFormat 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


