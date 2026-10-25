---
title: "Prj.Company"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트가 생성된 회사입니다."
type: docs
weight: 120
url: /ko/net/aspose.tasks/prj/company/
---
## Prj.Company field

프로젝트가 생성된 회사.

```csharp
public static readonly Key<string, PrjKey> Company;
```

## 예제

Prj.Company 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.Company, "Aspose");

Console.WriteLine("Company: " + project.Get(Prj.Company));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


