---
title: "Prj.ExtendedCreationDate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj field. 계산 및 보고에 사용되는 날짜"
type: docs
weight: 320
url: /ko/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

계산 및 보고에 사용되는 날짜.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## 예제

Prj.ExtendedCreationDate 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


