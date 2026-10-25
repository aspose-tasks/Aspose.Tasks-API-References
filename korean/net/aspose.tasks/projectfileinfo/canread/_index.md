---
title: "ProjectFileInfo.CanRead"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectFileInfo 속성. 프로젝트 파일을 Aspose.Tasks가 처리할 수 있는지 여부를 나타내는 값을 가져옵니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Aspose.Tasks가 프로젝트 파일을 처리할 수 있는지 여부를 나타내는 값을 가져옵니다.

```csharp
public bool CanRead { get; }
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

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


