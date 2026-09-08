---
title: "Prj.InsertedProjectsLikeSummary"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 하위 작업이 요약 작업으로 계산되는지 여부를 결정합니다."
type: docs
weight: 390
url: /ko/net/aspose.tasks/prj/insertedprojectslikesummary/
---
## Prj.InsertedProjectsLikeSummary field

하위 작업을 요약 작업으로 계산할지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> InsertedProjectsLikeSummary;
```

## 예제

Prj.InsertedProjectsLikeSummary 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.InsertedProjectsLikeSummary, true);

Console.WriteLine("Inserted Projects Like Summary: " + project.Get(Prj.InsertedProjectsLikeSummary));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


