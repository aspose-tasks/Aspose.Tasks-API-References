---
title: "Prj.FyStartDate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 회계 연도가 시작되는 월"
type: docs
weight: 350
url: /ko/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

회계 연도가 시작되는 월.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
```

## 예제

회계 연도 속성을 쓰는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// 회계 연도 속성을 설정합니다
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// 회계 연도 속성을 표시합니다
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


