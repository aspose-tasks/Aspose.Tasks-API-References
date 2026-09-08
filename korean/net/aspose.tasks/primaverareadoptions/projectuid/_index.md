---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraReadOptions 속성. 여러 프로젝트가 포함된 파일에서 읽을 프로젝트의 UID를 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

여러 프로젝트가 포함된 파일에서 읽을 프로젝트의 UID를 가져오거나 설정합니다.

```csharp
public int ProjectUid { get; set; }
```

## 예제

여러 프로젝트가 포함된 Primavera XML 또는 Primavera XER 파일에서 프로젝트를 읽는 방법을 보여줍니다.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// 특수 UID를 가진 프로젝트를 반환합니다.
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### 또 보기

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


