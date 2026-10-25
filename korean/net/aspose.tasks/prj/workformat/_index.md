---
title: "Prj.WorkFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 작업 기간을 표시하는 데 사용되는 형식"
type: docs
weight: 790
url: /ko/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

작업 기간을 표시하는 데 사용되는 형식.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## 예제

기본 작업 형식으로 기간을 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// 프로젝트의 기본 작업 형식으로 작업 값을 생성합니다
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


