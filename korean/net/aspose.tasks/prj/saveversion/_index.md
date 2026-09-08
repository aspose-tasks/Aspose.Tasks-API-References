---
title: "Prj.SaveVersion"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트 파일이 저장된 Microsoft Office Project 버전"
type: docs
weight: 620
url: /ko/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

프로젝트 파일이 저장된 Microsoft Office Project 버전.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## 예제

Shows how to check project's save version and save date.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// 프로젝트 버전 표시
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


