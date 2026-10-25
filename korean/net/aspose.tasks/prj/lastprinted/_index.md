---
title: "Prj.LastPrinted"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트의 마지막 인쇄 시간. mpp 파일에 UTC 형식으로 저장됩니다. DateTime 유형"
type: docs
weight: 430
url: /ko/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

프로젝트의 마지막 인쇄 시간. mpp 파일에 UTC 형식으로 저장됩니다. DateTime 형식.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## 예제

Prj.LastPrinted 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


