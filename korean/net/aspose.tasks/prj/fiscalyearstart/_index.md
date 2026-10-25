---
title: "Prj.FiscalYearStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 회계 연도 번호 매김을 사용할지 여부를 결정합니다"
type: docs
weight: 340
url: /ko/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

회계 연도 번호 매기기를 사용할지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


