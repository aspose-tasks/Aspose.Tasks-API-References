---
title: "Prj.Keywords"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트 키워드"
type: docs
weight: 410
url: /ko/net/aspose.tasks/prj/keywords/
---
## Prj.Keywords field

프로젝트의 키워드.

```csharp
public static readonly Key<string, PrjKey> Keywords;
```

## 예제

프로젝트 메타 정보를 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// 프로젝트 정보를 설정합니다
project.Set(Prj.Author, "Author");
project.Set(Prj.LastAuthor, "Last Author");
project.Set(Prj.Revision, 15);
project.Set(Prj.Keywords, "MSP Aspose");
project.Set(Prj.Comments, "Comments");

Console.WriteLine(project.Get(Prj.Author));
Console.WriteLine(project.Get(Prj.LastAuthor));
Console.WriteLine(project.Get(Prj.Revision));
Console.WriteLine(project.Get(Prj.Keywords));
Console.WriteLine(project.Get(Prj.Comments));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


