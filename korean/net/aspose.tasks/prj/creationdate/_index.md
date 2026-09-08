---
title: "Prj.CreationDate"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트가 생성된 날짜와 시간"
type: docs
weight: 130
url: /ko/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

프로젝트가 생성된 날짜와 시간.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## 비고

mpp 파일에 UTC 형식으로 저장됩니다. DateTime 형식.

## 예제

Shows how to read/write Prj.CreationDate property.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


