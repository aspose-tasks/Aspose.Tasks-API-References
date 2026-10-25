---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectFileInfo 속성. 프로젝트 파일 형식을 가져옵니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

프로젝트 파일 형식을 가져옵니다.

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


