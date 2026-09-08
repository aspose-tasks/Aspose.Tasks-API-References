---
title: "Prj.Subject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트의 주제"
type: docs
weight: 700
url: /ko/net/aspose.tasks/prj/subject/
---
## Prj.Subject field

프로젝트의 주제.

```csharp
public static readonly Key<string, PrjKey> Subject;
```

## 예제

Prj.Subject 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.Subject, "Subject");

Console.WriteLine("Subject: " + project.Get(Prj.Subject));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


