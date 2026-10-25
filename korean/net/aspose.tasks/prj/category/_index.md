---
title: "Prj.Category"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트의 카테고리"
type: docs
weight: 100
url: /ko/net/aspose.tasks/prj/category/
---
## Prj.Category field

프로젝트의 카테고리.

```csharp
public static readonly Key<string, PrjKey> Category;
```

## 예제

Prj.Category 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.Category, "Special");

Console.WriteLine("Category: " + project.Get(Prj.Category));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


