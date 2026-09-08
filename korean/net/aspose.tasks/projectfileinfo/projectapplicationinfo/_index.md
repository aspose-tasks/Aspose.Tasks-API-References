---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectFileInfo 속성. 프로젝트 파일 애플리케이션 정보를 가져옵니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

프로젝트 파일 애플리케이션 정보를 가져옵니다.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
```

## 예제

프로젝트 파일 정보를 읽는 방법을 보여줍니다.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 또 보기

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


