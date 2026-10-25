---
title: "Prj.LastSaved"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트가 마지막으로 저장된 날짜. mpp 파일에 UTC 형식으로 저장됩니다. DateTime 형식"
type: docs
weight: 440
url: /ko/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

프로젝트가 마지막으로 저장된 날짜. mpp 파일에 UTC 형식으로 저장됩니다. DateTime 형식.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


